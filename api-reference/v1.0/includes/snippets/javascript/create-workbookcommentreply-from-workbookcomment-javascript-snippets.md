---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0dc33799b0cace1cef0fcb9459b4be81bae483fe
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50794160"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookCommentReply = {
  content: 'This is my reply to the comment.',
  contentType: 'plain'
};

await client.api('/drive/items/{id}/workbook/comments/{id}/replies')
    .post(workbookCommentReply);

```