---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 306701cc24ebc55cca01502e42f6b1fc28706cf45087ac9e7ade5c3586a4a20e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105073"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookCommentReply = await client.api('/drive/items/{id}/workbook/comments/{id}/replies/{id}')
    .get();

```