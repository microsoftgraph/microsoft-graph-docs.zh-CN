---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 38adc03ea6da3dec86083cab2f5057b4e8a5d261
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50773226"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const unifiedGroupSource = {
  'group@odata.bind': '/groups/000044f9-47c8-4a87-bccf-291fbf006a54',
  includedSources: 'mailbox, site'
};

await client.api('/compliance/ediscovery/cases/{caseId}/custodians/{custodianId}/unifiedGroupSources')
    .version('beta')
    .post(unifiedGroupSource);

```