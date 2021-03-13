---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ea1bd567b54a031f3a8fab465a587fc8efcff94d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50801930"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/groups/{id}/removeFavorite')
    .version('beta')
    .post();

```