---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 457f3a0a518a752aab3411903aa7d4e6fe41eb868cf352085e996c2aea04bd0d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219217"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let int32 = await client.api('/groups/{id}/transitiveMembers/$count')
    .version('beta')
    .header('ConsistencyLevel','eventual')
    .get();

```