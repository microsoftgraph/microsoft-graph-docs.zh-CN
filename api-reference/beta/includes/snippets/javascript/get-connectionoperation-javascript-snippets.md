---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 31f7f88ae1e0b1c65446fded39636df485727673
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60694938"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let connectionOperation = await client.api('/external/connections/contosohr/operations/3ed1595a-4bae-43c2-acda-ef973e581323')
    .version('beta')
    .get();

```