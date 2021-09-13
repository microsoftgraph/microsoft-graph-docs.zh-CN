---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4f8e844bdcdef15e5644230d592c233153eac284db98f5f0555f35d9260f73a1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161182"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let personAward = await client.api('/me/profile/awards/{id}')
    .version('beta')
    .get();

```