---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e14632f06f2e2d3af83314bbe637831e799c3fc6
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66446700"
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

await client.api('/security/cases/eDiscoverycases/b0073e4e-4184-41c6-9eb7-8c8cc3e2288b/legalHolds/0053a61a3b6c42738f7606791716a22a/siteSources')
    .version('beta')
    .post(siteSource);

```