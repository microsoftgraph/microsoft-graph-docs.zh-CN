---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d6f0a5730e14a2620afdbc6f51630a89119da8d7
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48606412"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/messages')
    .select('sender,subject')
    .get();

```