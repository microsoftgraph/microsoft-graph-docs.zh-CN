---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 026d4c6e071596d183722e873509586d336f5b6e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50808827"
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