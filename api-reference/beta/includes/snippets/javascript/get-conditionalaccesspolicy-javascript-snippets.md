---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cd3b7b715e76974556da2d0a80e8b8d9954d84126393d6d696d3e4b31556412c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221132"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let conditionalAccessPolicy = await client.api('/identity/conditionalAccess/policies/{id}')
    .version('beta')
    .get();

```