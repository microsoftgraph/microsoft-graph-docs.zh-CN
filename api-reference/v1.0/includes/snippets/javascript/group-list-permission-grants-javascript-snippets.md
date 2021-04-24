---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b1228a093619346fd8d221de6ace97e5a0430772
ms.sourcegitcommit: 2006bf01c60793ac6ab1e25fa0526ec5d33c6334
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/23/2021
ms.locfileid: "51961392"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let permissionGrants = await client.api('/groups/14c981a4-dca9-4565-bae6-e13ada8861be/permissionGrants')
    .get();

```