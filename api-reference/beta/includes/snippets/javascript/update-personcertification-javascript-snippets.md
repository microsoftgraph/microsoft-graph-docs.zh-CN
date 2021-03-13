---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 80c9d6f80150c4bd6369d0548c650635ccfa8bc1
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50774584"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const personCertification = {
  issuingAuthority: 'International Academy of Marketing Excellence',
  issuingCompany: 'International Academy of Marketing Excellence'
};

await client.api('/users/{userId}/profile/certifications/{id}')
    .version('beta')
    .update(personCertification);

```