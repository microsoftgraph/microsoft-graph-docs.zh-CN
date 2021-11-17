---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4468625fce1f613c0f092825ba8201798d69cf50b96b6d9b3c0d2fa70fe235fc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162912"
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