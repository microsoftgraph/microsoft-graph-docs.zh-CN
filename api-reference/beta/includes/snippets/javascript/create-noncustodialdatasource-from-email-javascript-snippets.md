---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 732388c3fe262baa7475152c7817549bf2681408
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "60927047"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const noncustodialDataSource = {
    applyHoldToSource: true,
    dataSource: {
        '@odata.type': 'microsoft.graph.ediscovery.userSource',
        email: 'adelev@contoso.com'
    }
};

await client.api('/compliance/ediscovery/cases/5b840b94-f821-4c4a-8cad-3a90062bf51a/noncustodialDataSources')
    .version('beta')
    .post(noncustodialDataSource);

```