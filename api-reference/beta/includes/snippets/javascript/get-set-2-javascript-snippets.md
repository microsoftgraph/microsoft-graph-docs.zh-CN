---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9ff657146d26b8baf3ae08212e89dec7f4d6e92e
ms.sourcegitcommit: 5bb981b4853663354a566d4a4a5cbf288939e441
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2021
ms.locfileid: "53580473"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let set = await client.api('/termStore/sets/8ed8c9ea-7052-4c1d-a4d7-b9c10bffea6f')
    .version('beta')
    .get();

```