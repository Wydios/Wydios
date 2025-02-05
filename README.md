
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
        youtube: '@wydios',
        twitch: '@wydios',
        discord: '@wydios',
        tiktok: '@wydios'
    };
    return { name, user, age, socials, };
};
