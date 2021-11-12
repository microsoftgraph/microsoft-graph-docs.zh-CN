---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d4d99f6bfd1a99444014348ef622fb35b91a7a50ef6efb2d832e7be69b49f8b6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104729"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let shifts = await client.api('/teams/{teamId}/schedule/shifts')
    .version('beta')
    .filter('sharedShift/startDateTime ge 2019-03-11T00:00:00.000Z and sharedShift/endDateTime le 2019-03-18T00:00:00.000Z and draftShift/startDateTime ge 2019-03-11T00:00:00.000Z and draftShift/endDateTime le 2019-03-18T00:00:00.000Z')
    .get();

```