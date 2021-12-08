---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8fec039ef33f136d2a23a4e761c3a5130db794aa
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2021
ms.locfileid: "61341813"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const accessPackage = {
  displayName: 'sales reps',
  description: 'outside sales representatives',
  isHidden: false,
  catalog: {
    id: '66584aae-98bb-48cc-9458-7bee5d2a6577'
  }
};

await client.api('/identityGovernance/entitlementManagement/accessPackages')
    .post(accessPackage);

```