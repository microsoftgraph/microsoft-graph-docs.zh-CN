---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6c55783f6de0194052b9eebd763a65f6499ad7e0
ms.sourcegitcommit: 4e16f26b6b685a6a3dae855a04979c84105609b9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/10/2022
ms.locfileid: "62519616"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const accessPackageCatalog = {
  displayName: 'Catalog One'
};

await client.api('/identityGovernance/entitlementManagement/catalogs/{accessPackageCatalogId}')
    .update(accessPackageCatalog);

```