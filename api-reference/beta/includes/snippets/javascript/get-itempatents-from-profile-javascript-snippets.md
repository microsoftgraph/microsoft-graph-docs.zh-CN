---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9a49d1fc315c61424212f8912df82da38842df4665ed23fe8a9faea24a2f218a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106871"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let patents = await client.api('/me/profile/patents')
    .version('beta')
    .get();

```