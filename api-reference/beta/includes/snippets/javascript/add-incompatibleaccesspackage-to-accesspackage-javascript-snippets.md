---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 79c0739703f53d62f1636410f86bf10246267252
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439829"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const accessPackage = {
    '@odata.id': 'https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/c0a74b4d-2694-4d5d-a964-1bee4ff0aaf2'
};

await client.api('/identityGovernance/entitlementManagement/accessPackages/{id}/incompatibleAccessPackages/$ref')
    .version('beta')
    .post(accessPackage);

```