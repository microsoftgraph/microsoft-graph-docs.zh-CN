---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9a7af29d851133ee9fd8b4733df87e92f6a1a2a4
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35731399"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}?expand=fields')
    .get();

```