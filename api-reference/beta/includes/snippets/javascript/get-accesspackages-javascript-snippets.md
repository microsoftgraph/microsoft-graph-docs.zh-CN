---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f4c308c3fcb96c7350ee26af12de89eb796b8c25
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50795718"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let accessPackages = await client.api('/identityGovernance/entitlementManagement/accessPackages')
    .version('beta')
    .get();

```