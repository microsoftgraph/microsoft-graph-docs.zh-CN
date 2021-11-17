---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 40eaba0ead62b969c8e994d1668f9c9fec25d2bff60fbfb0918c06926a9d7a36
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273996"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let identityUserFlow = await client.api('/identity/userFlows/B2C_1_Pol1')
    .version('beta')
    .get();

```