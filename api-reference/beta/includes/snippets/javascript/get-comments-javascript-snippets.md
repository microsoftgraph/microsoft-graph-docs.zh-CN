---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: de0fddb5b9ef255760f1db7d7415e1950ef26bfb
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50784053"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let comments = await client.api('/drive/items/{id}/workbook/comments')
    .version('beta')
    .get();

```