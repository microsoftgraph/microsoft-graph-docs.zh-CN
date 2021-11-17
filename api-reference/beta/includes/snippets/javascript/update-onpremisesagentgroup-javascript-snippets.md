---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3d6b97779a6d8f8b4364a2a2efcfb928daf734570f376f2e3fa86cb4651f8485
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57103862"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const onPremisesAgentGroup = {
    displayName: 'Group New Name'
};

await client.api('/onPremisesPublishingProfiles/provisioning/agentGroups/8832388F-3814-4952-B288-FFB62081FE25/')
    .version('beta')
    .update(onPremisesAgentGroup);

```