---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a99fd5cd2f260cbeb1ce6f53dc66b8748fca8270
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50950450"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let sets = await client.api('/termStore/groups/{groupId}/sets')
    .version('beta')
    .get();

```