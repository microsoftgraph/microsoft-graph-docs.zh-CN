---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5227f3d053e8cfffc8ad3c12262d182ad5da7ba12506b53c7ec7d85aba8c356c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101418"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/deviceManagement/virtualEndpoint/onPremisesConnections/{id}')
    .version('beta')
    .delete();

```