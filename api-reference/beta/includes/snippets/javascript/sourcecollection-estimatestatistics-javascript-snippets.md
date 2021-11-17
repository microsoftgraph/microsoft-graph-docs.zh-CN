---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 722d7e6d77fdec6e6e6744a639c52f0414d6d46dcf1aa0f0a2be86f8dbaea7f1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274401"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}/estimateStatistics')
    .version('beta')
    .post();

```