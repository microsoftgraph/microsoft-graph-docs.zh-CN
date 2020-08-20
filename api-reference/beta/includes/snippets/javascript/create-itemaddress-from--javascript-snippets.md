---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c02d668e10afd511dc03a651ddff2acf412d473a
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/20/2020
ms.locfileid: "46820228"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const itemAddress = {
  displayName: "Home",
  detail: {
    type: "home",
    postOfficeBox: null,
    street: "221B Baker Street",
    city: "London",
    state: null,
    countryOrRegion: "United Kingdom",
    postalCode: "E14 3TD"
  }
};

let res = await client.api('/me/profile/addresses')
    .version('beta')
    .post(itemAddress);

```