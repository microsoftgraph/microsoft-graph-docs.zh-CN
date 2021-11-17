---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0c8061f03240768596a77faea9ef1c786ca4b17a9e2eb12515813037a44c1fee
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215826"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let offerShiftRequests = await client.api('/teams/{teamId}/schedule/offerShiftRequests')
    .version('beta')
    .get();

```