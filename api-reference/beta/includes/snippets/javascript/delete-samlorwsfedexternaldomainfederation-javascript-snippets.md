---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2d0ec7a0b1e7880ee038b775f720d2da99baf47e
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59765006"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/directory/federationConfigurations/96db02e2-80c1-5555-bc3a-de92ffb8c5be')
    .version('beta')
    .delete();

```