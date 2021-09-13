---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 50a94be27747ada9d14e217c64de699af2e4d3450ceadd961d2a6ea64757ce76
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220859"
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