---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cc954290e2f5510b8c901c55bb4417e55e304949
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66440212"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const dataSource = {
    '@odata.type': 'microsoft.graph.security.siteSource',
    site: {
        webUrl: 'https://contoso.sharepoint.com/sites/SecretSite'
    }
};

await client.api('/security/cases/ediscoveryCases/{ediscoveryCaseId}/searches/{ediscoverySearchId}/additionalSources')
    .version('beta')
    .post(dataSource);

```