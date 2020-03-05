---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e19a2c13595d5e05d394bf9476d1619ccaa9e4e9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42440544"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/communications/callRecords/{id}')
    .version('beta')
    .expand('sessions($expand=segments)')
    .get();

```