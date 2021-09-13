---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fe19e0725a1b61ec29895eea6ff418cdddb4a9fdcc73f0fbe714d9cb443d9d23
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274102"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let teamsApps = await client.api('/appCatalogs/teamsApps')
    .filter('id eq \'b1c5353a-7aca-41b3-830f-27d5218fe0e5\'')
    .get();

```