---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1d3827d8b01e5bb987c0f9154bf9aad13fa42677edd2fa55663be106984efe32
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220886"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const itemPatent = {
  number: 'USPTO-3954432633',
  webUrl: 'https://patents.gov/3954432633'
};

await client.api('/users/{userId}/profile/patents/{id}')
    .version('beta')
    .update(itemPatent);

```