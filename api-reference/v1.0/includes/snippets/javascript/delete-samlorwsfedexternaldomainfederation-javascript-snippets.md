---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2d0ec7a0b1e7880ee038b775f720d2da99baf47e
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65315372"
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