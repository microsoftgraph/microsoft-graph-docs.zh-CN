---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6d864e777c0f1bcb3e0a99f0d4ba9124f6552e3f
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48616089"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/acceptedSenders')
    .get();

```