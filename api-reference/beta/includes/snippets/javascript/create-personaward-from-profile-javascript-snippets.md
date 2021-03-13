---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e4e262b507a8c008a1d1754ce09735d194992079
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50805558"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const personAward = {
  description: 'Lifetime Achievement award from the International Association of Branding Managers',
  displayName: 'Lifetime Achievement Award For Excellence in Branding',
  issuedDate: 'Date',
  issuingAuthority: 'International Association of Branding Management',
  thumbnailUrl: 'https://iabm.io/sdhdfhsdhshsd.jpg',
  webUrl: 'https://www.iabm.io'
};

await client.api('/me/profile/awards')
    .version('beta')
    .post(personAward);

```