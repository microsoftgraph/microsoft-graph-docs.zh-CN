---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eb4777865d5fd5c8e53c98a591f677dfe1aa9b6c
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66092453"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const siteSource = {
    site: {
        webUrl: 'https://m365x809305.sharepoint.com/sites/Retail'
    }
};

await client.api('/security/cases/eDiscoverycases/b0073e4e-4184-41c6-9eb7-8c8cc3e2288b/custodians/0053a61a3b6c42738f7606791716a22a/siteSources')
    .version('beta')
    .post(siteSource);

```