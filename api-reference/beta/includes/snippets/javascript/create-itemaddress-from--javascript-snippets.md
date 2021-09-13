---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c16ec6301b85fdfbf4663ce221a7f48016408ef5baa5fc249aa1ed72fc25a558
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378403"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const itemAddress = {
  displayName: 'Home',
  detail: {
    type: 'home',
    postOfficeBox: null,
    street: '221B Baker Street',
    city: 'London',
    state: null,
    countryOrRegion: 'United Kingdom',
    postalCode: 'E14 3TD'
  }
};

await client.api('/me/profile/addresses')
    .version('beta')
    .post(itemAddress);

```