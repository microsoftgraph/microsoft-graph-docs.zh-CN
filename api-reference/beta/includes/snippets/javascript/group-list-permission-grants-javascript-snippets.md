---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eca59f1495d2b6c029e3eab2e3284ef27e3233c180d44a1dd30b0f0e722061b3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903418"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let permissionGrants = await client.api('/groups/14c981a4-dca9-4565-bae6-e13ada8861be/permissionGrants')
    .version('beta')
    .get();

```