---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6248ca7cb40fa1aa903c5586da948b8701e3400359df5c3d7934f128eb046ba5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277261"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let namedLocations = await client.api('/identity/conditionalAccess/namedLocations')
    .filter('createdDateTime ge 2019-09-01T00:00:00Z')
    .get();

```