---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 60486a4f458ddbf3a27e98bbaf61e6c5e756f09bb42ee8f41097d02d26936399
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903087"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let history = await client.api('/riskyUsers/41a31b00-3b3b-42d9-8f1c-6d4f14e74c69/history')
    .version('beta')
    .get();

```