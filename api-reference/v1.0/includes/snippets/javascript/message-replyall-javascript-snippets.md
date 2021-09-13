---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 216f3c3c2b55caf8dcff1c02d161ca15d8b7f02c82fd679601801c9919b456d7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409025"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const replyAll = {
  comment: 'comment-value'
};

await client.api('/me/messages/{id}/replyAll')
    .post(replyAll);

```