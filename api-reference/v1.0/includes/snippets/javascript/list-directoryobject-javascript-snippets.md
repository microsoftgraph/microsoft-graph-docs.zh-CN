---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e64c6ccfdb51310aa3d96d46f8b9d8c66d253c67
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62137616"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let internalSponsors = await client.api('/identityGovernance/entitlementManagement/assignments/{accessPackageAssignmentId}/target/connectedOrganization/internalSponsors')
    .get();

```