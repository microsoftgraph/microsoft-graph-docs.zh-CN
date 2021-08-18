---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d0d350a13e72974a84cf8809448bf1613dcff6045c44080ac9819ada36d59246
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378588"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let users = await client.api('/users')
    .version('beta')
    .filter('startswith(displayName,\'Eric\')')
    .select('displayName,signInActivity')
    .get();

```