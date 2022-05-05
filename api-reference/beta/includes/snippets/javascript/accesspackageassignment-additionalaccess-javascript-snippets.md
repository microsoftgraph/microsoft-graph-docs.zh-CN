---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 308fc025b0954e1fe963b0dfe6a82501dd1e2c56
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65203791"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let additionalAccess = await client.api('/identityGovernance/entitlementManagement/accessPackageAssignments/additionalAccess(accessPackageId='2506aef1-3929-4d24-a61e-7c8b83d95e6f',incompatibleAccessPackageId='d5d99728-8c0b-4ede-83d2-cf9b0e8dabfb')')
    .version('beta')
    .expand('target')
    .get();

```