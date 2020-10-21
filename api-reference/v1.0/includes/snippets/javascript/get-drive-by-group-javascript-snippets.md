---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b86a51f5011660b609ea853b58eb49bce2cb13e8
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48615557"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{groupId}/drive')
    .get();

```