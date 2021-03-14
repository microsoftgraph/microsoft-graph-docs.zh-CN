---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b32e51f196d159c5240bf5ee90d111d5970ca8d8
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50784263"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/contacts/{id}')
    .delete();

```