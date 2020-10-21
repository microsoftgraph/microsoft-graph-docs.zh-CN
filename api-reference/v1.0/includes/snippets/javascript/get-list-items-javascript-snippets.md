---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0123bec184b2f1f0145b109bef7016ec6a9856d4
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48605623"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Name,Color,Quantity)')
    .get();

```