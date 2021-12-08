---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1935912eb68919ca310af24b31e432f7808cc4e8
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2021
ms.locfileid: "61335249"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let externalSponsors = await client.api('/identityGovernance/entitlementManagement/assignments/{accessPackageAssignmentId}/target/connectedOrganization/externalSponsors')
    .get();

```