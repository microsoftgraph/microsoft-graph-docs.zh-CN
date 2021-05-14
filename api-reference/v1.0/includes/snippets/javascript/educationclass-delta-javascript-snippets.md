---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8fd059549cfac3306d9d1062c8d86266c9048f20
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "52475026"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delta = await client.api('/education/classes/delta')
    .get();

```