---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5ddb5182449dcf083fa91a34e2ebe26d67120f8a
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48606886"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/calendarGroups')
    .get();

```