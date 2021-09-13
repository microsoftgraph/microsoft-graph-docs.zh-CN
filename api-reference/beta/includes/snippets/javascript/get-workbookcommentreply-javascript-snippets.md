---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 196513c566844d5ed9dfa57c2c3772025c8722e00da4728abcfb6d46f5ac091f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278259"
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