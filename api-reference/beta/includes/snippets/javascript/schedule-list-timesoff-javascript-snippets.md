---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4786ab2997d243c1559a8af4f5c1b3a4e336c8cae1b55c54d78014af04b97628
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378639"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let timesOff = await client.api('/teams/{teamId}/schedule/timesOff')
    .version('beta')
    .filter('sharedTimeOff/startDateTime ge 2019-03-11T00:00:00.000Z and sharedTimeOff/endDateTime le 2019-03-18T00:00:00.000Z and draftTimeOff/startDateTime ge 2019-03-11T00:00:00.000Z and draftTimeOff/endDateTime le 2019-03-18T00:00:00.000Z')
    .get();

```