---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f36cb0e1b179dcc1ecd74c9a99ccc42661e82679714f3742f5be1b71d215e64f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279632"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let names = await client.api('/me/profile/names')
    .version('beta')
    .get();

```