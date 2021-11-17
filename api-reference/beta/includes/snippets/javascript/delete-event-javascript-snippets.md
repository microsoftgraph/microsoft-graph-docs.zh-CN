---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 47071d6608772ee1a0e06f13c6ce414b4846533c906b53db1fc5f042e3a52029
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106147"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/events/{id}')
    .version('beta')
    .delete();

```