---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2efdfe3f98964312fd615f604ac086aa399034b3
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636873"
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
    .post(device);

```