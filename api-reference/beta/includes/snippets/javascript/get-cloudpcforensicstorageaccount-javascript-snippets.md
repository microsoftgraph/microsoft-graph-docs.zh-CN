---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 503d3da5569857e0bc2a12c7b1daae71adfa7a50
ms.sourcegitcommit: 1d9193fa91f44d80ecdc2b82e37272df1c9630f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/22/2022
ms.locfileid: "65629357"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let getStorageAccounts = await client.api('/deviceManagement/virtualEndpoint/snapshots/getStorageAccounts(subscriptionId='cb6ad4c4-8a17-4245-a644-e4436b1ee204')')
    .version('beta')
    .get();

```