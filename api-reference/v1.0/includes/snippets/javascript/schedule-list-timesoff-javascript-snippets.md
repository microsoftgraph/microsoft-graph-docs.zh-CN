---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 09849a6e6759205f8a095f4c97f05fffad253ac8
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50779408"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let timesOff = await client.api('/teams/{teamId}/schedule/timesOff')
    .filter('sharedTimeOff/startDateTime ge 2019-03-11T00:00:00.000Z and sharedTimeOff/endDateTime le 2019-03-18T00:00:00.000Z and draftTimeOff/startDateTime ge 2019-03-11T00:00:00.000Z and draftTimeOff/endDateTime le 2019-03-18T00:00:00.000Z')
    .get();

```