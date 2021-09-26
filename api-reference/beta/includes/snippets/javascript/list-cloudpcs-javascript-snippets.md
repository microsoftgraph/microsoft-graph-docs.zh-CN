---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6672fecc3185cd8bb10d58322401a86f906e5b4a1a028a0ecdc82d8c66547d98
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106848"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let cloudPCs = await client.api('/deviceManagement/virtualEndpoint/cloudPCs')
    .version('beta')
    .get();

```