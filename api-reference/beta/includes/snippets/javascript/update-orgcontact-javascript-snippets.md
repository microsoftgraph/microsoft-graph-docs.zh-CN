---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 034a69581acbaa246195b8d58577391c666a346c50eb9f11c7da4bc4fd3530eb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163671"
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