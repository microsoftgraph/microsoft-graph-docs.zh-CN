---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a68ec91295b8277b5cf0fdb2917c3ec3c36d251c7b6eae59c04ac552e45cf480
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104199"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let accessPackageAssignments = await client.api('/identityGovernance/entitlementManagement/accessPackageAssignments')
    .version('beta')
    .get();

```