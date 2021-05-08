---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a586e48b7a23401ae77f0f0b19e68b2774791780
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52254241"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const unifiedGroupSource = {
  'group@odata.bind': 'https://graph.microsoft.com/v1.0/groups/b96f95c5-b1b3-4142-b039-8ac79e7d2c84',
  includedSources: 'mailbox, site'
};

await client.api('/compliance/ediscovery/cases/{caseId}/custodians/{custodianId}/unifiedGroupSources')
    .version('beta')
    .post(unifiedGroupSource);

```