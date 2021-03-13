---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4eb4c0a78a280e4a63468568e97ee44720116175
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50798650"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let connectedOrganization = await client.api('/identityGovernance/entitlementManagement/connectedOrganizations/{id}')
    .version('beta')
    .get();

```