---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9fd2455bc56536696def422680c9cf598c1232be21df22f3ced2f5012c4cc75e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274262"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let user = await client.api('/groups/{id}/transitiveMembers/microsoft.graph.user')
    .header('ConsistencyLevel','eventual')
    .search('displayName:tier')
    .select('displayName,id')
    .orderby('displayName')
    .get();

```