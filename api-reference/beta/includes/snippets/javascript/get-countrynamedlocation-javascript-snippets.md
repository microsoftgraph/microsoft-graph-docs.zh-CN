---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f6de4d377470df8d2be97b060f0d60461f13c76a
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37937128"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/conditionalAccess/namedLocations/1c4427fd-0885-4a3d-8b23-09a899ffa959')
    .version('beta')
    .get();

```