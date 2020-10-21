---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bde22c2f046a5613790f83d81094d081d1d9dbb5
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48616363"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/reminderView(startDateTime='2017-06-05T10:00:00.0000000',endDateTime='2017-06-11T11:00:00.0000000')')
    .get();

```