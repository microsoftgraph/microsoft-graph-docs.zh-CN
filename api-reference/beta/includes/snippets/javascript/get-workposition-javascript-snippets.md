---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9e74085a82211a530070bb4ccd07ddb59077af49252fe084b048db4980c0106c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163195"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workPosition = await client.api('/me/profile/positions/{id}')
    .version('beta')
    .get();

```