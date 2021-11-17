---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 160cd02921ec068d1d29f7a349514718f7c265a6815126f271cedbac8e0fc42c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219445"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let conditionalAccessPolicyCoverages = await client.api('/tenantRelationships/managedTenants/conditionalAccessPolicyCoverages')
    .version('beta')
    .get();

```