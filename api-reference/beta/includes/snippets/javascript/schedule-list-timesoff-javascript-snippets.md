---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c51f8f8193d4538b0ae0a86a9b461f7d92c26807
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35725644"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teams/{teamId}/schedule/timesOff')
    .version('beta')
    .filter('sharedTimeOff/startDateTime ge 2019-03-11T00:00:00.000Z and sharedTimeOff/endDateTime le 2019-03-18T00:00:00.000Z and draftTimeOff/startDateTime ge 2019-03-11T00:00:00.000Z and draftTimeOff/endDateTime le 2019-03-18T00:00:00.000Z')
    .get();

```