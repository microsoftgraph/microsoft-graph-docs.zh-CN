---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 455df61bf929bb1ce5c377567444b74833b67aef2f8af344695288a8be4e4fab
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105144"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let educationUser = await client.api('/education/users/13012')
    .version('beta')
    .get();

```