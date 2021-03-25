---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a26b2918abb24a487e7c2c8e39fe0f491db2bd59
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51201046"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let columns = await client.api('/sites/{site-id}/lists/{list-id}/columns')
    .version('beta')
    .get();

```