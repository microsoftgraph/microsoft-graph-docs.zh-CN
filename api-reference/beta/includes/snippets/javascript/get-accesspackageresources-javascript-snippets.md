---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2139fc87f3d80b1499b2c1219099e704ddbb8c5f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50791559"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let accessPackageResources = await client.api('/identityGovernance/entitlementManagement/accessPackageCatalogs/{id}/accessPackageResources')
    .version('beta')
    .get();

```