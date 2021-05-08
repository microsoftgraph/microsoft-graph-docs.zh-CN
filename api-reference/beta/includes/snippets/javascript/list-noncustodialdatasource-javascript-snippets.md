---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f60b57475c4d33d7cded29dfb7ec6f7cdfe37664
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52240794"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let noncustodialSources = await client.api('/compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}/noncustodialSources')
    .version('beta')
    .get();

```