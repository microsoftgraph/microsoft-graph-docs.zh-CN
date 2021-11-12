---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d9de055756ab24042cb152ef0374dd62caa8c8c42dc776310c239736480a5826
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219070"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let contract = await client.api('/contracts/{id}')
    .version('beta')
    .get();

```