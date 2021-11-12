---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 909fb3df695bd9e0ea16a22195864ab129fd338ccacb4b443d78c9b61022b542
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277286"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let printTask = await client.api('/print/taskDefinitions/3203656e-6069-4e10-8147-d25290b00a3c/tasks/d036638b-1272-4bba-9227-732463823ed3')
    .version('beta')
    .get();

```