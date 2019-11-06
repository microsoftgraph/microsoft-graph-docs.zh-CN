---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b6a37eb2d6b9893fabaa5b06907de33fb845cd4a
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994117"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const accessPackage = {
  catalogId: "aa2f6514-3232-46e7-a08a-2411ad8d7128",
  displayName: "sales reps",
  description: "outside sales representatives"
};

let res = await client.api('/identityGovernance/entitlementManagement/accessPackages')
    .version('beta')
    .post(accessPackage);

```