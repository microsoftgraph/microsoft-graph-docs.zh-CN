---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 57b3add8444a66fe6d5d02bfa17b7763fc1f02cd3a4ff4c9af1a18dd1342f5a2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57328918"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let onPremisesPublishingProfile = await client.api('/onPremisesPublishingProfiles/provisioning')
    .version('beta')
    .expand('agentGroups')
    .get();

```