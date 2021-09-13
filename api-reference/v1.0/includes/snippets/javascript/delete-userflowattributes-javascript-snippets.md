---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: abccecb256ac049be83f5d8809f7b2908e1a7d3d3021b8471ce65d36fde43862
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161618"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/identity/userFlowAttributes/extension_d09380e2b4c642b9a203fb816a04a7ad_Hobby')
    .delete();

```