---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d7e7f4f3332f4f0fe7014634a3d0a384f3f05dfa
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2021
ms.locfileid: "61340693"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let connectedOrganization = await client.api('/identityGovernance/entitlementManagement/connectedOrganizations/04e7fa5f-fa5f-04e7-5ffa-e7045ffae704')
    .get();

```