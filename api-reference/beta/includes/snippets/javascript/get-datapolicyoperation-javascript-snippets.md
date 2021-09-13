---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 95f6c0e0f0ceccb0a303c6e1fcfdeed1e65e573afc85b394e6ecd01d253d78ab
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162273"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let dataPolicyOperation = await client.api('/dataPolicyOperations/{id}')
    .version('beta')
    .get();

```