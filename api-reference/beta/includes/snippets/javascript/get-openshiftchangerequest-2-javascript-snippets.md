---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a5e3cc473c1bc6a1a5dacbc0d266d8c3ef9a947c0eafb112e95d592d8cd2bc65
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106518"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let openShiftChangeRequests = await client.api('/teams/{id}/schedule/openShiftChangeRequests')
    .version('beta')
    .get();

```