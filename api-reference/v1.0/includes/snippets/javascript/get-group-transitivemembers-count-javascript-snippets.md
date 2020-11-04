---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c060dbc100008ef29b047ca76be16113953b5a74
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48904830"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/transitiveMembers/$count')
    .header('ConsistencyLevel','eventual')
    .get();

```