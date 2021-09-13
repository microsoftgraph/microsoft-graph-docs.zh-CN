---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8f1667ed9c186bd618a93fc54a19a6555f911cadbb6be51d40e8463ae0a5322f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220504"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/users/{userId}/profile/addresses/{id}')
    .version('beta')
    .delete();

```