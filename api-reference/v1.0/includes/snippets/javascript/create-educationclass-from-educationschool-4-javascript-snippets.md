---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 34c13057c4a8920b68cae0b261c1afda630063df
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50956589"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/education/schools/{school-id}/users/{user-id}')
    .delete();

```