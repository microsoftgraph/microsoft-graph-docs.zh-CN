---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c47422a90bb26d4889ac787f17a48cb6a80d7dec
ms.sourcegitcommit: 64d27a0e3dcccc9d857e62aace4153e5d98fb3d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60736655"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookCommentReply = await client.api('/me/drive/items/{id}/workbook/comments/{id}/replies/{id}')
    .get();

```