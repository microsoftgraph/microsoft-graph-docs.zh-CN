---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: de631a34b03c2aa6142c903712f201eaea5f0b8f
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63336793"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const user = {
  addLicenses: [
    {
      disabledPlans: [ '11b0131d-43c8-4bbb-b2c8-e80f9a50834a' ],
      skuId: '45715bb8-13f9-4bf6-927f-ef96c102d394'
    }
  ],
  removeLicenses: [ 'bea13e0c-3828-4daa-a392-28af7ff61a0f' ]
};

await client.api('/me/assignLicense')
    .post(user);

```