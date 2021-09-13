---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 39d2157ed19b5647a345f5a8797a3c3a7fc2822653ce1fd017f3eee5c1a769f0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278921"
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