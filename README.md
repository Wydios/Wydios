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
        youtube: '[@wydios](https://www.youtube.com/@Wydios)',
        twitch: '[@wydios](https://www.twitch.tv/wydios)',
        tiktok: '[@wydios](https://www.tiktok.com/@wydios)',
        discord: '@wydios'
    };

    return { name, user, age, socials };
};
