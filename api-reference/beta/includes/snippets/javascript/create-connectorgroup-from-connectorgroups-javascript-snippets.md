---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 15227a427f31f6d95a7e4d7f179accd75ebd76533a1904c30a00f0f5431d76a5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57103887"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const connectorGroup = {
  name: 'name-value',
  isDefault: false
};

await client.api('/onPremisesPublishingProfiles/applicationProxy/connectorGroups')
    .version('beta')
    .post(connectorGroup);

```