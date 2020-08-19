---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ab710bafe0032f766a03a0232875fece095584c7
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46806404"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const accessPackageCatalog = {
  displayName:"Catalog One"
};

let res = await client.api('/identityGovernance/entitlementManagement/accessPackageCatalogs/{accessPackageCatalogId}')
    .version('beta')
    .update(accessPackageCatalog);

```