---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9abfe8e8843c0e916973d638b2b85ccacd7e25c6
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "60927056"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const noncustodialDataSource = {
    applyHoldToSource: false,
    dataSource: {
        '@odata.type': 'microsoft.graph.ediscovery.siteSource',
        site: {
            webUrl: 'https://contoso.sharepoint.com/sites/SecretSite'
        }
    }
};

await client.api('/compliance/ediscovery/cases/15d80234-8320-4f10-96d0-d98d53ffdfc9/noncustodialdatasources')
    .version('beta')
    .post(noncustodialDataSource);

```