---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 347089775c3d90ed8a0f245ef808fb48c018bf80c6c2711358221920e0fd0cf7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903622"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let tokenIssuancePolicy = await client.api('/policies/tokenIssuancePolicies/{id}')
    .version('beta')
    .get();

```