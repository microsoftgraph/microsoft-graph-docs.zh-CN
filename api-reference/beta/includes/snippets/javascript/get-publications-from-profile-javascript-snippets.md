---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d8945e74fad6db8edb9872683d9313e85b368eaca84c8f73a8641209506a9f64
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333181"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let publications = await client.api('/me/profile/publications')
    .version('beta')
    .get();

```