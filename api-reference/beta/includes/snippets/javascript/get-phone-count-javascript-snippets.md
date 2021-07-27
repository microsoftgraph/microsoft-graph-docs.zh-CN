---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fdd944b587ed989843b8b6088f53e1200da909d8
ms.sourcegitcommit: 5bb981b4853663354a566d4a4a5cbf288939e441
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2021
ms.locfileid: "53580975"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let contacts = await client.api('/contacts')
    .version('beta')
    .header('ConsistencyLevel','eventual')
    .search('displayName:wa')
    .get();

```