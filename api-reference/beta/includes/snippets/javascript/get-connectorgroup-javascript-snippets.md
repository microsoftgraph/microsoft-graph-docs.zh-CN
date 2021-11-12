---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 01bee839ff425da4322cc01f94c6a23ea85c2e46f61c41c8e02daa8cd93d3547
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57328808"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let connectorGroup = await client.api('/onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}')
    .version('beta')
    .get();

```