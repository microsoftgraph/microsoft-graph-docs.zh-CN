---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 19dc88ce1d43dbd87f517937fe4c22c909661d44
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50805982"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/contactFolders/{id}')
    .version('beta')
    .delete();

```