---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 29971cd2ec7e992d82773e063af50cc656702ebbb5168743361a15db02402b43
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902891"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let phoneMethods = await client.api('/me/authentication/phoneMethods')
    .version('beta')
    .get();

```