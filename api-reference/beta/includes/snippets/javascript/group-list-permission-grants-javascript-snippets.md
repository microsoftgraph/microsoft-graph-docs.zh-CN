---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fda3e0613e64f5c391e87fdcef4b61d01b3b2cf3
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2021
ms.locfileid: "51611359"
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