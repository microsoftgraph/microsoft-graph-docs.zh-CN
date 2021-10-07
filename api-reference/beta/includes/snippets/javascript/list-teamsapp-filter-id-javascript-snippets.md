---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 537f0ca02b4fdf1d65b7e4dd90e8427612e50471660f784fe7f0e723c048d16e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215719"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let teamsApps = await client.api('/appCatalogs/teamsApps')
    .version('beta')
    .filter('id eq \'b1c5353a-7aca-41b3-830f-27d5218fe0e5\'')
    .get();

```