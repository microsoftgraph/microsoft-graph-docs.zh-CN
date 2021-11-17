---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a4f0dbfb1d3d37811f7ca377c30331b283bf04910b55239c155d1475489eb23e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163723"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let namedLocations = await client.api('/identity/conditionalAccess/namedLocations')
    .version('beta')
    .filter('createdDateTime ge 2019-09-01T00:00:00Z')
    .get();

```