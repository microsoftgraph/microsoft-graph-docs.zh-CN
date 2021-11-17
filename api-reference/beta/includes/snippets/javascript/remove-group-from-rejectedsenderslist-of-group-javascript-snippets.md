---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 44c5ac74104816f468ae12a66b07a755a10a3263a4511de17ab46ce58839123e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277319"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/groups/{id}/rejectedSenders/$ref')
    .version('beta')
    .delete();

```