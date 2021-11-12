---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0c940050ce95b958b33141ccd9646be154d7c24a353e9101a72558144118a2ee
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163244"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let connectorGroups = await client.api('/onPremisesPublishingProfiles/applicationProxy/connectorGroups')
    .version('beta')
    .get();

```