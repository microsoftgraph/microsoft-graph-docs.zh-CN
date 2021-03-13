---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e3fbf543b578d13b790c591a62acf2ccb781ea7e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800150"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let driveItemVersion = await client.api('/me/drive/items/{item-id}/versions/{version-id}')
    .version('beta')
    .get();

```