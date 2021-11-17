---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c849fe941d205af0ee1dc4f88985d02cf7d3edfbcdeb97a3b630f8a6881ec31a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105808"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}')
    .version('beta')
    .delete();

```