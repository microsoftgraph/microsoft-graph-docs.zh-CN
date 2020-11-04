---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3ae15777a283d8a302bfc1d186f0100eb1ef96c5
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48905795"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const certificateBasedAuthConfiguration = {
  certificateAuthorities: [
    {
      isRootAuthority: true,
      certificate: "Binary"
    }
  ]
};

let res = await client.api('/organization/{id}/certificateBasedAuthConfiguration/$ref')
    .post(certificateBasedAuthConfiguration);

```