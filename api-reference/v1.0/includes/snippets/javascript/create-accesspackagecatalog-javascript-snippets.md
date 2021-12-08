---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0553b32cfe8477c8c679ef35dff6ec5495added9
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2021
ms.locfileid: "61335484"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const accessPackageCatalog = {
  displayName: 'sales',
  description: 'for employees working with sales and outside sales partners',
  state: 'published',
  isExternallyVisible: true
};

await client.api('/identityGovernance/entitlementManagement/catalogs')
    .post(accessPackageCatalog);

```