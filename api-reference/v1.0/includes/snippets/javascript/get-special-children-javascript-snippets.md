---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 098b05fb70ca4e59db47c0d5996093523972b8c2
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50789764"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let children = await client.api('/me/drive/special/{special-folder-name}/children')
    .get();

```