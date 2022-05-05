---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0ff027a5f0f37cd85eb09dba17a1fa30adb18f07
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65211435"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}/purgeData')
    .version('beta')
    .post();

```