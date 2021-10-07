---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1ccbf120260df89c5c679b348c9126102db306fb5f0b2b84c95bed0c7e702847
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215718"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let teamsApps = await client.api('/appCatalogs/teamsApps')
    .version('beta')
    .filter('externalId eq \'cf1ba4c7-f94e-4d80-ba90-5594b641a8ee\'')
    .get();

```