```js
class About {
    constructor() {
        this.name = 'Fabian';
        this.user = 'Wydios';
        this.age = 16;
        this.today = new Date();
        
        if (this.isBirthday(9, 3)) {
            this.age++;
        }

        this.socials = {
            youtube: '@wydios Link: https://www.youtube.com/@Wydios',
            twitch: '@wydios Link: https://www.twitch.tv/wydios',
            tiktok: '@wydios Link: https://www.tiktok.com/@wydios',
            discord: '@wydios Link: https://discord.gg/7ngxfFYxY4'
        };
    }

    isBirthday(month, day) {
        return this.today.getMonth() === month && this.today.getDate() === day;
    }

    getInfo() {
        return {
            name: this.name,
            user: this.user,
            age: this.age,
            socials: this.socials
        };
    }
}
const aboutMe = new About();
