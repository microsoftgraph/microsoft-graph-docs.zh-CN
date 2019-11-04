---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e8a2f187277a065f3783455a004286ae1c272c7d
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938501"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/conditionalAccess/namedLocations/0854951d-5fc0-4eb1-b392-9b2c9d7949c2')
    .version('beta')
    .delete();

```