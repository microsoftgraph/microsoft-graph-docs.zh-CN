---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b67274f9555c5001b03b62c40e2ff1b900bbfa3d718895377a9c52e39064e9a2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218598"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/contacts/{id}')
    .version('beta')
    .delete();

```