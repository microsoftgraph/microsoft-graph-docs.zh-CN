---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 542cff86ce73dd1ab5f8d41151894f280afa07d2881677627c2708ed2269059e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277177"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let categories = await client.api('/education/classes/a17025d0-62a8-4450-9e6e-db31d8c8feb8/assignments/1fdf61ee-c129-4960-9b7c-8df159aa64b0/categories')
    .get();

```