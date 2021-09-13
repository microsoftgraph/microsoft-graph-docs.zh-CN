---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ddf07857a8fa3fc677748dba2dac63b3c5556715ceaf6cf81d461b352723fa28
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162381"
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