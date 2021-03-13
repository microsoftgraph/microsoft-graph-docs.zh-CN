---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cb7c6f0c9213deb021aab41b7e33fa456253f701
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50799373"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delta = await client.api('/contacts/delta')
    .version('beta')
    .select('displayName,jobTitle,mail')
    .get();

```