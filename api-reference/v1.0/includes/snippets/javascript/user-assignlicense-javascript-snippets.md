---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0edb8ddbf3dbfb3bf3a2d1f8009806f574deaf2cf147f6c3077abc83ea3e6076
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104921"
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
      skuId: 'guid'
    }
  ],
  removeLicenses: [ 'bea13e0c-3828-4daa-a392-28af7ff61a0f' ]
};

await client.api('/me/assignLicense')
    .post(user);

```