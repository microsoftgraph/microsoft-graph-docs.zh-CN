---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 150237901e6ca373953973dd0a1821f64a07516b51f778bbedaafccf80787eda
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162486"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let identityApiConnector = await client.api('/identity/apiConnectors/{id}')
    .version('beta')
    .get();

```