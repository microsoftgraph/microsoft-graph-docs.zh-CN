---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c2c146ac6e5319f3c78f313edcba5309e88bd9f6
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34481014"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationClass = {
  description: "Health Level 1",
  classCode: "Health 501",
  displayName: "Health 1",
  externalId: "11019",
  externalName: "Health Level 1",
  externalSource: "sis",
  mailNickname: "fineartschool.net"
};

let res = await client.api('/education/classes')
    .version('beta')
    .post({educationClass : educationClass});

```