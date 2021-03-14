---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 600586ff0d18be536c48d1659d07f5f612480805
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50786700"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let shifts = await client.api('/teams/{teamId}/schedule/shifts')
    .filter('sharedShift/startDateTime ge 2019-03-11T00:00:00.000Z and sharedShift/endDateTime le 2019-03-18T00:00:00.000Z and draftShift/startDateTime ge 2019-03-11T00:00:00.000Z and draftShift/endDateTime le 2019-03-18T00:00:00.000Z')
    .get();

```