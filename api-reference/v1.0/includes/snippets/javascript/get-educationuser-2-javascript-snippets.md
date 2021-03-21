---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 53d5c9c156c0bd8117c2a49b1627dd5548d60282
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50963693"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let educationUser = await client.api('/education/users/{user-id}')
    .get();

```