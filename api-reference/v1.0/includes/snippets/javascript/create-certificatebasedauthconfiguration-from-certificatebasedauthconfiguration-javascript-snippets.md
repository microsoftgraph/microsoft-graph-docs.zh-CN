---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dc4f5af2cf32996038d418f57f6e9b88b363d6b9
ms.sourcegitcommit: 22bd45d272681658d46a8b99af3c3eabc7b05cb1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/18/2021
ms.locfileid: "58385523"
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
      certificate: 'Binary'
    }
  ]
};

await client.api('/organization/{id}/certificateBasedAuthConfiguration')
    .post(certificateBasedAuthConfiguration);

```