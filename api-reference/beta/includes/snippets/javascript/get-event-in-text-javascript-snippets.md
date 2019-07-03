---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ff53c433ca80cdb6219a3f588021c674c10ade7f
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35499581"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/events/AAMkAGI1AAAoZDOFAAA=/')
    .version('beta')
    .header('Prefer','outlook.body-content-type="text"')
    .select('subject,body,bodyPreview')
    .get();

```