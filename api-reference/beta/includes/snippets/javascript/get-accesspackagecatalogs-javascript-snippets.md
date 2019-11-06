---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5d83fff7a2562c4bec294d9be478c7c7424a8a80
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994242"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/identityGovernance/entitlementManagement/accessPackageCatalogs')
    .version('beta')
    .get();

```