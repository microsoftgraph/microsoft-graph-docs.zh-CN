---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 36e00024ea2c59c908a21604018fc15bc8e90341
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50805291"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let photos = await client.api('/groups/{id}/photos')
    .version('beta')
    .get();

```