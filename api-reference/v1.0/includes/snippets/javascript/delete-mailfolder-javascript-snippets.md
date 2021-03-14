---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e41b28cb0323e6d7ecf6dc6ea1a1785d6ced6bbd
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50788355"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/mailFolders/{id}')
    .delete();

```