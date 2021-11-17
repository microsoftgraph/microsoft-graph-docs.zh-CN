---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8b62639bf5d50f51e8b8dc283815fcbbb8f96663af323da39a3edca7c8787c13
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277385"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let usageRights = await client.api('/users/{userId}/usageRights')
    .version('beta')
    .get();

```