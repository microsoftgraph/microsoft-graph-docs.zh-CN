---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e5d3e45cae234a9131ce07b20cbb6e4a881f72b4
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48605558"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/messages/{id}/createReply')
    .post();

```