---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b9f6074a44f9cc9fbc08460628e2c9977227150441930ec1d13dd28bdaf4b065
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332886"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/onPremisesPublishingProfiles/provisioning/agentGroups/8832388F-3814-4952-B288-FFB62081FE25/')
    .version('beta')
    .delete();

```