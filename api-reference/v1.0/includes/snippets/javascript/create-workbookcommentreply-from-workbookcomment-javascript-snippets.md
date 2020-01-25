---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 627dd12386547d937517e6ddc7ff8a8fe37afb21
ms.sourcegitcommit: 2f78ac96a9b0462626a242429055ef824590bd3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2020
ms.locfileid: "41497688"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookCommentReply = {
  content: "This is my reply to the comment.",
  contentType: "plain"
};

let res = await client.api('/drive/items/{id}/workbook/comments/{id}/replies')
    .post(workbookCommentReply);

```