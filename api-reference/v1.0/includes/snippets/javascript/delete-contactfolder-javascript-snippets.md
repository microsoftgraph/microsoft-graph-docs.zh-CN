---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e5eae858f09b686d53a3e22a25194448caedab9a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50791043"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/contactFolders/{id}')
    .delete();

```