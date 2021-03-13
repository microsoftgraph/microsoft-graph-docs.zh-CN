---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bf89b013966e3013944c5a0d6cb0d300bb586e5d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50773275"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let string = await client.api('/compliance/ediscovery/cases/99e865fc-e29f-479a-ba83-9e58eb017103/operations/63926d4779c243458902328d83f61f53/microsoft.graph.ediscovery.caseExportOperation/getDownloadUrl')
    .version('beta')
    .get();

```