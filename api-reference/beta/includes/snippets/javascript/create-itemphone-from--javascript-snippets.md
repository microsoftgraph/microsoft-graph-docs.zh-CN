---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ae0e025fae5fe9737da1ab0e644d4498cd7af205
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/20/2020
ms.locfileid: "46819792"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const itemPhone = {
  displayName: "Car Phone",
  number: "+7 499 342 22 13"
};

let res = await client.api('/me/profile/phones')
    .version('beta')
    .post(itemPhone);

```