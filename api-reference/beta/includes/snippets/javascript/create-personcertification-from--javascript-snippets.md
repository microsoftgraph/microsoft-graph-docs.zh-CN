---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: acec6a7750ef2a5a33ea315200141bd030b2e116
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/20/2020
ms.locfileid: "46820195"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const personCertification = {
  certificationId: "KB-1235466333663322",
  description: "Blackbelt in Marketing - Brand Management",
  displayName: "Marketing Blackbelt - Brand Management",
  thumbnailUrl: "https://iame.io/dfhdfdfd334.jpg",
  webUrl: "https://www.iame.io/blackbelt"
};

let res = await client.api('/me/profile/certifications')
    .version('beta')
    .post(personCertification);

```