---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d95c05fd38f2b75afc33be3548734b9e19116175
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2021
ms.locfileid: "61342438"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let connectedOrganizations = await client.api('/identityGovernance/entitlementManagement/connectedOrganizations')
    .get();

```