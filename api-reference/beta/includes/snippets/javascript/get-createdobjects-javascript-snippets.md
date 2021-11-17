---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9b7459a40eedfcce7bc43cfa03628f26e8fef56b20b5510eab753914b7e2176e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218441"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let createdObjects = await client.api('/me/createdObjects')
    .version('beta')
    .get();

```