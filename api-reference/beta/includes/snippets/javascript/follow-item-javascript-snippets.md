---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0e10168b55ee00cd2975b0d7f359d8f17da3f47f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50794950"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/drive/items/{item-id}/follow')
    .version('beta')
    .post();

```