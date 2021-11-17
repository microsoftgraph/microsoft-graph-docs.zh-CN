---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e8f57e2da86254c8b48fe28cf804021d2adda6881774f336c847410bd0fef3d4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56904215"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let permission = await client.api('/sites/{sitesId}/permissions/{permissionId}')
    .version('beta')
    .get();

```