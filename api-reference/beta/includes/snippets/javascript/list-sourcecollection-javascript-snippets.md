---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f326dd9b8701956050fc2fee9a99413d8357c0d1
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50776583"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let sourceCollections = await client.api('/compliance/ediscovery/cases/{caseId}/sourceCollections')
    .version('beta')
    .get();

```