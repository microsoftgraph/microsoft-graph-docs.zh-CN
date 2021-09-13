---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1dbb990ed87f1cae684eecb585729e438fa206fb75067b1f85912d226cc88572
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56904295"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let schemaExtension = await client.api('/schemaExtensions/graphlearn_test')
    .get();

```