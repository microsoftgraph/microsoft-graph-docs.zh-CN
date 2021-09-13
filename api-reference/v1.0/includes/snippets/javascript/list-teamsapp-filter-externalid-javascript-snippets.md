---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: da94f7e0552838ed568d2ead31ff6357166254ba99eb45e52900b157c323c81e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274101"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let teamsApps = await client.api('/appCatalogs/teamsApps')
    .filter('externalId eq \'cf1ba4c7-f94e-4d80-ba90-5594b641a8ee\'')
    .get();

```