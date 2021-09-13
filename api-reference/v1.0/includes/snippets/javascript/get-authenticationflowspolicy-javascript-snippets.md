---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5c05b87041c7841354b3c883050abe4435f2e0fc892db1f8d0f6ab10bc0a55fa
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903560"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let authenticationFlowsPolicy = await client.api('/policies/authenticationFlowsPolicy')
    .get();

```