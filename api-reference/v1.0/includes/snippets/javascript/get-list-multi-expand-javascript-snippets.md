---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2f57caff9f3f9fd1ff700f94a25ef830afe942e5
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50782801"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let list = await client.api('/sites/{site-id}/lists/{list-id}?select=id,name,lastModifiedDateTime&expand=columns(select=name,description),items(expand=fields(select=Name,Color,Quantity))')
    .get();

```