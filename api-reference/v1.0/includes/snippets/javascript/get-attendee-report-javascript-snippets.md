---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3208f72826276571db41758a9c10aa5411f64707
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/01/2022
ms.locfileid: "65820863"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let stream = await client.api('/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZiMi04ZdFpHRTNaR1F6WGhyZWFkLnYy/attendeeReport')
    .get();

```