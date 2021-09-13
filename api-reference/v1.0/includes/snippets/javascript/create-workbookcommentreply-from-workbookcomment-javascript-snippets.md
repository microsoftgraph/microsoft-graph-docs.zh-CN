---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bcdef74fa3b8fe9924dda5146442603ac26702fa51e5a4269b826fcada88c875
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57328832"
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