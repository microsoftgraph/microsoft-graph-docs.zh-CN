---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bdfac26f9f07b54c37bdb5b5a1ef5eb1c0272f4a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50784081"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let labels = await client.api('/me/informationProtection/policy/labels')
    .version('beta')
    .get();

```