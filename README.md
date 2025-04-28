```ts
type AboutInfo = {
    name: string;
    user: string;
    age: number;
    socials: SocialLinks;
};

type SocialLinks = {
    youtube: string;
    twitch: string;
    tiktok: string;
    discord: string;
};

function About(): AboutInfo {
    const name = 'Fabian';
    const user = 'Wydios';
    let age = 16;
    const today = new Date();

    function isBirthday(month: number, day: number): boolean {
        return today.getMonth() === month && today.getDate() === day;
    }

    if (isBirthday(9, 3)) {
        age++;
    }

    const socials: SocialLinks = {
        youtube: "https://www.youtube.com/@Wydios",
        twitch: "https://www.twitch.tv/wydios",
        tiktok: "https://www.tiktok.com/@wydios",
        discord: "https://discord.gg/7ngxfFYxY4"
    };

    return { name, user, age, socials };
};

const { name, user, age, socials } = About();
console.log(`Hello, I am ${user}, a German guy. My real name is ${name},
I am ${age} years old. You can follow me on my socials ➜
• YouTube: ${socials.youtube}
• Twitch: ${socials.twitch}
• TikTok: ${socials.tiktok}
• Discord Server: ${socials.discord}`);
