---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 95a6ac778661e3ae64195528eba8c3c8f7a5353e
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35466919"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const device = {
  accountEnabled:false,
  alternativeSecurityIds:
  [
    {
      type:2,
      key:"base64Y3YxN2E1MWFlYw=="
    }
  ],
  deviceId:"4c299165-6e8f-4b45-a5ba-c5d250a707ff",
  displayName:"Test device",
  operatingSystem:"linux",
  operatingSystemVersion:"1"
};

let res = await client.api('/devices')
    .post({device : device});

```