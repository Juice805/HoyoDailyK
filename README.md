## How to use
1. Fork this repo. For the links below to work properly, you need to follow this help from <ins>your</ins> forked repo.
2. Get your **LTUID** and **LTOKEN** values from HoYoLAB
   * **LTUID** is just your HoYoLAB user ID. It can be found on **[Account info](https://www.hoyolab.com/accountCenter)** page under your username or in the URL
   * **LTOKEN** is a browser cookie used to authenticate yourself to HoYoLAB. Obtaining it is a little trickier:
     * Go to **[HoYoLAB](https://www.hoyolab.com)** and make sure you are logged in
     * Press `Ctrl`+`Shift`+`I` or just `F12` to open developer tools
     * Open Application tab, under Storage section expand Cookies and select `https://www.hoyolab.com`
     * Using search you can find both **LTUID** and **LTOKEN** keys  
       ![image](https://user-images.githubusercontent.com/40900803/148886385-f373c064-f961-408b-8eea-0ebee76806bc.png)
3. Add them to your repo's **[Secrets](../../settings/secrets/actions/new)**
4. Go to **[Actions](../../actions)** and enable them,
   then open **[the workflow](../../actions/workflows/sign-in.yml)** and enable it too
5. _(Optional)_ If you want to sign-in right now,
   go to **[Actions > HoYoLAB Daily Sign-in](../../actions/workflows/sign-in.yml)** and run workflow.

### Warning
If you change your HoYoLAB password, **LTOKEN** value changes too. Don't forget to update it!
