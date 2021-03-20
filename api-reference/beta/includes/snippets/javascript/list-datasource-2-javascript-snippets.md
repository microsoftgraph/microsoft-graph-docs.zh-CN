---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 859c59451fec8bfc52e7f1ce6f10ccb3fce349a1
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50952107"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let custodianSources = await client.api('/compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}/custodianSources')
    .version('beta')
    .get();

```