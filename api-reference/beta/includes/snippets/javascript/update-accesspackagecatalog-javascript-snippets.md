---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cd9481e34cb42bf9c8230dd4767733810f5e2953
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50799665"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const accessPackageCatalog = {
  displayName: 'Catalog One'
};

await client.api('/identityGovernance/entitlementManagement/accessPackageCatalogs/{accessPackageCatalogId}')
    .version('beta')
    .update(accessPackageCatalog);

```