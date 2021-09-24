---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 84bdb6380d69ef85b61f788a7932d2df4dbca44d
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59507372"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let categories = await client.api('/education/classes/f4a941ff-9da6-4707-ba5b-0eae93cad0b4/assignments/9018ae7a-9953-4796-a152-4c54e0910922/categories')
    .version('beta')
    .get();

```