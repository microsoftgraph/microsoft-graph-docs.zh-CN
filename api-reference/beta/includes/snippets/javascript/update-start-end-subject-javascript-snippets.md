---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f9ee55100db95305a1fd741be506bdde379638eeaf1435d6d1f4552c117e1867
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219951"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const onlineMeeting = {
  startDateTime: '2020-09-09T14:33:30.8546353-07:00',
  endDateTime: '2020-09-09T15:03:30.8566356-07:00',
  subject: 'Patch Meeting Subject'
};

await client.api('/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZi')
    .version('beta')
    .update(onlineMeeting);

```