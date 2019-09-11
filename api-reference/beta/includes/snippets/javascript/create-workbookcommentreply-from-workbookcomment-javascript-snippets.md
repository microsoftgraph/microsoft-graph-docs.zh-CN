---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 80a2111fff11bbde5d83a6294808c23fb74d9066
ms.sourcegitcommit: d8a58221ed1f2b7b7073fd621da4737e11ba53c5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/11/2019
ms.locfileid: "36838915"
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

let res = await client.api('/drive/root/workbook/comments/{id}/replies')
    .version('beta')
    .post(workbookCommentReply);

```