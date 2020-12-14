---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a225a8704dea3e6d53bc7cf1827faf36a133d30e
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/11/2020
ms.locfileid: "49659044"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const unifiedGroupSource = {
  group@odata.bind: "/groups/000044f9-47c8-4a87-bccf-291fbf006a54",
  includedSources:  "mailbox, site"
};

let res = await client.api('/compliance/ediscovery/cases/{ediscoveryCaseId}/custodians/{custodianId}/unifiedGroupSources')
    .version('beta')
    .post(unifiedGroupSource);

```