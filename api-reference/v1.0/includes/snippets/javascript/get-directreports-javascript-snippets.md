---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0234838742ff96c8e927c235ecdc772a130bde0a
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48617521"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/directReports')
    .get();

```