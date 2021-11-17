---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 48e0212f8e914411cdea5370e4869e67aba2a7a63ea1ed62103ace04fbc3e3a6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163619"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let teamsAppIcon = await client.api('/appCatalogs/teamsApps/95de633a-083e-42f5-b444-a4295d8e9314/appDefinitions/OTVkZTYzM2EtMDgzZS00MmY1LWI0NDQtYTQyOTVkOGU5MzE0IyMxLjAuNSMjUHVibGlzaGVk/outlineIcon/')
    .version('beta')
    .get();

```