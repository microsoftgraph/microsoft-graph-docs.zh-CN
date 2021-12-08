---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5034d0cb27067b5fd1c37cbfa06d35b3a008cd17
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2021
ms.locfileid: "61341802"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let accessPackage = await client.api('/identityGovernance/entitlementManagement/accessPackages/114d3459-3459-114d-5934-4d1159344d11')
    .get();

```