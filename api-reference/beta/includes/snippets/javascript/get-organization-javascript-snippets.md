---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 022f799d26171c9486231a5a4b8f8c68952b46c1
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50793558"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let organization = await client.api('/organization')
    .version('beta')
    .get();

```