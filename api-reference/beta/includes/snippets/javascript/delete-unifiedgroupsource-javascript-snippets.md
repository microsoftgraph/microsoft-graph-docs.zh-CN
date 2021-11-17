---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4768310b968d2556f68da7a24bd01e5993fa1fcc5371c863978997e058fa4bc1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105156"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/compliance/ediscovery/cases/{caseId}/custodians/{custodianId}/unifiedGroupSources/{unifiedGroupSourceId}')
    .version('beta')
    .delete();

```