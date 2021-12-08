---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2213847f2c2ec2de2a70d80baa97af67bd8729ec
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2021
ms.locfileid: "61346212"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let catalogs = await client.api('/identityGovernance/entitlementManagement/catalogs')
    .get();

```