---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2cef370643b48e2c15d663c1552d33b25945c352
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994215"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const accessPackageCatalog = {
  displayName: "sales",
  description: "for employees working with sales and outside sales partners",
  isExternallyVisible: true
};

let res = await client.api('/identityGovernance/entitlementManagement/accessPackageCatalogs')
    .version('beta')
    .post(accessPackageCatalog);

```