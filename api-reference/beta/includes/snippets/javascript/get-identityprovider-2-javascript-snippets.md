---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 978a703d925a548b44c53199ce4e0309f3c1a997f0e53caac0fa80c2ef9b9a75
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163808"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let identityProvider = await client.api('/identityProviders/{id}')
    .version('beta')
    .get();

```