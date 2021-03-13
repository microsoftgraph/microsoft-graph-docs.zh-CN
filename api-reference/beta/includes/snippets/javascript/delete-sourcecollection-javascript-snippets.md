---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ab488399ac2c3384dd3182c019ac6a5446fdc4e0
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50772763"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}')
    .version('beta')
    .delete();

```