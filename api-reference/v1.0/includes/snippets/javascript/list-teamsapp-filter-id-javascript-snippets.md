---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c41394949f3b98f13e2c3190937a9aee99331071
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50774857"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let teamsApps = await client.api('/appCatalogs/teamsApps')
    .filter('id eq \'b1c5353a-7aca-41b3-830f-27d5218fe0e5\'')
    .get();

```