```js
function About() {
    const name = 'Fabian';
    const user = 'Wydios';
    let age = 16;
    const today = new Date();

    const isBirthday = (date, month, day) =>
        date.getMonth() === month && date.getDate() === day;

    if (isBirthday(today, 9, 3)) {
        age++;
    }

    const socials = {
        youtube: '@wydios Link: https://www.youtube.com/@Wydios',
        twitch: '@wydios Link: https://www.twitch.tv/wydios',
        tiktok: '@wydios Link: https://www.tiktok.com/@wydios',
        discord: '@wydios Link: https://discord.gg/7ngxfFYxY4'
    };

    return { name, user, age, socials };
};
