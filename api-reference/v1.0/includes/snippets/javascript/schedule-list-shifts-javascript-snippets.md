---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9eda9b033403b550dd6fa8c8c2eb8bbb892947fe552c1b6b4a448ea05a6db720
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162540"
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