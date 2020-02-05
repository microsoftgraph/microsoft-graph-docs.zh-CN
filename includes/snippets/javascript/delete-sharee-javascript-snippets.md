---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e16ece06f20d74d57ebc7cbc9809dac3f4e3791b
ms.sourcegitcommit: 7b286637aa332cfd534a41526950b4f6272e0fd7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/05/2020
ms.locfileid: "41774804"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users/AlexW@contoso.OnMicrosoft.com/calendars/AAMkADAwAABf02bAAAA=/calendarPermissions/L289RXhjaGFuZ2VMYWJTWVnYW5C')
    .version('beta')
    .delete();

```