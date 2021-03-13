---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a6cd572e40130f6d195b9b4af2f3c613597645ee
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50798550"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const orgContact = {
  businessPhones: [
    'businessPhones-value'
  ],
  city: 'city-value',
  companyName: 'companyName-value',
  country: 'country-value',
  department: 'department-value',
  displayName: 'displayName-value'
};

await client.api('/contacts/{id}')
    .version('beta')
    .update(orgContact);

```