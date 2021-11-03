---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2a72b2c5fbb1da396032d1ea3b3eb044311c3f6f
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60696750"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/external/connections/contosohr')
    .version('beta')
    .delete();

```