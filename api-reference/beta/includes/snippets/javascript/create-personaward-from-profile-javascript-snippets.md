---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3b4c401ecf9b05933937e9ae6795d99602373820
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/20/2020
ms.locfileid: "46819564"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const personAward = {
  description: "Lifetime Achievement award from the International Association of Branding Managers",
  displayName: "Lifetime Achievement Award For Excellence in Branding",
  issuedDate: "Date",
  issuingAuthority: "International Association of Branding Management",
  thumbnailUrl: "https://iabm.io/sdhdfhsdhshsd.jpg",
  webUrl: "https://www.iabm.io"
};

let res = await client.api('/me/profile/awards')
    .version('beta')
    .post(personAward);

```