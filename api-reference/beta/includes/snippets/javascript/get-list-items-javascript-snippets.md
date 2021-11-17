---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 88a9f994a6d9e542d70b253db3cb6f315c177f11bc7222c3037d4d19085e6e2b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158530"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let items = await client.api('/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Name,Color,Quantity)')
    .version('beta')
    .get();

```