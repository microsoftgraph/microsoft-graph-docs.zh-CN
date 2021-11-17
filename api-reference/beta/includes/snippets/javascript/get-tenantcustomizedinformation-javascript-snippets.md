---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d8176b35ec4a43b00a466f301ff22fd4ce96e3afb9d6cf7c42424d7c2067763e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161406"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let tenantCustomizedInformation = await client.api('/tenantRelationships/managedTenants/tenantsCustomizedInformation/{tenantCustomizedInformationId}')
    .version('beta')
    .get();

```