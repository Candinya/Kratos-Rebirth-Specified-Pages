---
title: 好伙伴们
date: 2018-08-06 12:44:02
comments: false
description: 好伙伴们在哪里~
---
<div class="linkpage"><ul id="friendsList"></ul></div>

// 以下为样例内容，按照格式可以随意修改
<script type="text/javascript">
{
    const myFriends = [
        ["#", "https://candinya.com/images/avatar.png", "猫猫", "喵喵~"],
        ["#", "https://candinya.com/images/avatar.png", "猫猫猫", "喵喵喵~"],
        ["#", "https://candinya.com/images/avatar.png", "猫猫猫猫", "喵喵喵喵~"]
    ];

    let friendNodes = '';
    while (myFriends.length > 0) {
        const rndNum = Math.floor(Math.random()*myFriends.length);
        friendNodes += `<li><a target="_blank" href="${myFriends[rndNum][0]}"><img src="${myFriends[rndNum][1]}"><h4>${myFriends[rndNum][2]}</h4><p>${myFriends[rndNum][3]}</p></a></li>`;
        myFriends.splice(rndNum, 1);
    }
    document.getElementById("friendsList").innerHTML = friendNodes;
}
</script>