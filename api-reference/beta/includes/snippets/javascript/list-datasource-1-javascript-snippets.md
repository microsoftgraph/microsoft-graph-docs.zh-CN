---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c2fe8be0fabb6d31edc5b7685d4ca452d81c1edd
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50952143"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let additionalSources = await client.api('/compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}/additionalSources')
    .version('beta')
    .get();

```