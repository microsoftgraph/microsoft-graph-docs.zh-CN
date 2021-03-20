---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c140bf1acccd2b8d1c1b499874385237be134f5f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50944246"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const group = {
  description: 'description-value',
  displayName: 'displayName-value',
};

await client.api('/groups/{id}')
    .version('beta')
    .update(group);

```