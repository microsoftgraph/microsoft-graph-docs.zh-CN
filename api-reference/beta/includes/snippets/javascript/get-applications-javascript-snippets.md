---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fcf4893288b5a5379b091c7deebe4cf0cf138cd85b7d5bf4c2e9ed873dd0c7e9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903440"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let applications = await client.api('/onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}/applications')
    .version('beta')
    .get();

```