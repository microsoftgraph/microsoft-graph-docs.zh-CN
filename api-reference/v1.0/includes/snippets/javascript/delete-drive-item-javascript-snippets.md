---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7b38d8b317077ce4e489f7b143193e3b6aeb2b57
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50803974"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/drive/items/{item-id}')
    .delete();

```