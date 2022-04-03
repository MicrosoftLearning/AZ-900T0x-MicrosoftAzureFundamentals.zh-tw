---
title: 線上託管說明
permalink: index.html
layout: home
ms.openlocfilehash: c8816b7d9de9c19fbd4c6b3f373d6e4336c6ca5a
ms.sourcegitcommit: 26c283fffdd08057fdce65fa29de218fff21c7d0
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/27/2022
ms.locfileid: "137907675"
---
# <a name="content-directory"></a>內容目錄

指向每個逐步解說的超連結。 講師可以選擇將逐步解說用作示範或學生實驗室。 

## <a name="walkthroughs"></a>逐步解說

{% assign wts = site.pages | where_exp:"page", "page.url contains '/Instructions/Walkthroughs'" %}
| 模組 | 逐步介紹 |
| --- | --- | 
{% for activity in wts %}| {{ activity.wts.module }} | [{{ activity.wts.title }}{% if activity.wts.type %} - {{ activity.wts.type }}{% endif %}]({{ site.github.url }}{{ activity.url }}) |
{% endfor %}

