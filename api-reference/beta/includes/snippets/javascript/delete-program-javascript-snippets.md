---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a0aa28c191ce4cc492b9b6b1a346d4f65eea8c5f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800394"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/programs/7e59d237-2fb0-4e5d-b7bb-d4f9f9129213')
    .version('beta')
    .delete();

```