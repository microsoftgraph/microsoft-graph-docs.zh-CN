---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e070d1cc02bdbd4e193635c410d32a6a1de5373f
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2020
ms.locfileid: "44219225"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teamwork/workforceIntegrations/{workforceIntegrationId}')
    .version('beta')
    .delete();

```