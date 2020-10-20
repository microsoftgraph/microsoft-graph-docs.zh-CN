---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f7c8e6748e86998b8ffc7c5cb21b3db22fa0b896
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48619185"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/tables')
    .version('beta')
    .get();

```