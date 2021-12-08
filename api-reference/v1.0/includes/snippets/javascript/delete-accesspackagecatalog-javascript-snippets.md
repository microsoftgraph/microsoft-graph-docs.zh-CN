---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 57a4374829e38812ee37f77155419b53b70b5b3a
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2021
ms.locfileid: "61346996"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/identityGovernance/entitlementManagement/catalogs/{accessPackageCatalogId}')
    .delete();

```