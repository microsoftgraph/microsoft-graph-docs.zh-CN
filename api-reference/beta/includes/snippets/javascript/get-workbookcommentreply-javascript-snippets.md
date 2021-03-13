---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b9e71110634cc826e524e5786a16af4f547c7785
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50796110"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookCommentReply = await client.api('/drive/items/{id}/workbook/comments/{id}/replies/{id}')
    .version('beta')
    .get();

```