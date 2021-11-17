---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c609b9bac76da4d8e24c7b624488840c1d86ee6a4b6653a93b740780f6e0cd2b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274024"
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
    .version('beta')
    .post(certificateBasedAuthConfiguration);

```