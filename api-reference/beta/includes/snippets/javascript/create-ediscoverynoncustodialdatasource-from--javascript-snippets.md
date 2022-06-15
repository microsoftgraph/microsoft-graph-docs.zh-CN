---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f3536e4bf3038cde45831be0d7b254c6f11237a7
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66092279"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const ediscoveryNoncustodialDataSource = {
    dataSource: {
        '@odata.type': 'microsoft.graph.security.siteSource',
        site: {
            webUrl: 'https://m365x809305.sharepoint.com/sites/Design-topsecret'
        }
    }
};

await client.api('/security/cases/eDiscoverycases/b0073e4e-4184-41c6-9eb7-8c8cc3e2288b/noncustodialDataSources')
    .version('beta')
    .post(ediscoveryNoncustodialDataSource);

```