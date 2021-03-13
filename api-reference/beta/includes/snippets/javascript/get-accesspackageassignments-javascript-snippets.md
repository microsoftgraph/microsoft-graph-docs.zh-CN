---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c8ebb696ca189a055c61a3db53e612dc2fccc075
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50797277"
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