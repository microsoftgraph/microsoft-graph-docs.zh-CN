---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ff90f0639281b6e4070ec2aaad388d320b07b944
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66096131"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const ediscoveryHoldPolicy = {
    displayname: 'My legalHold with sources',
    description: 'Created from Graph API',
    contentQuery: 'Bazooka',
    'userSources@odata.bind': [
        {
            '@odata.type': 'microsoft.graph.security.userSource',
            email: 'SalesTeam@M365x809305.OnMicrosoft.com'
        }
    ],
    'siteSources@odata.bind': [
        {
            '@odata.type': 'microsoft.graph.security.siteSource',
            site: {
                webUrl: 'https://m365x809305.sharepoint.com/sites/Design-topsecret'
            }
        }
    ]
};

await client.api('/security/cases/eDiscoverycases/b0073e4e-4184-41c6-9eb7-8c8cc3e2288b/legalHolds')
    .version('beta')
    .post(ediscoveryHoldPolicy);

```