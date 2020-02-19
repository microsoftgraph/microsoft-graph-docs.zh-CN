---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8b90e5bfbabb47d109d41b83a00ecb865123a962
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "37992919"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/identityGovernance/entitlementManagement/accessPackageAssignmentRequests')
    .version('beta')
    .get();

```