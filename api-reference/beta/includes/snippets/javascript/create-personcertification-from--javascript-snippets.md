---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: efe0e142a1139baf600e9e9d4524b9443d483413
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50788329"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const personCertification = {
  certificationId: 'KB-1235466333663322',
  description: 'Blackbelt in Marketing - Brand Management',
  displayName: 'Marketing Blackbelt - Brand Management',
  thumbnailUrl: 'https://iame.io/dfhdfdfd334.jpg',
  webUrl: 'https://www.iame.io/blackbelt'
};

await client.api('/me/profile/certifications')
    .version('beta')
    .post(personCertification);

```