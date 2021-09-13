---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 896727b79c08fcec3cdf11c62fb66dd3582a3392070c77cf892bc2e78eebc50f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903863"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delegatedPermissionClassifications = await client.api('/servicePrincipals/{id}/delegatedPermissionClassifications')
    .get();

```