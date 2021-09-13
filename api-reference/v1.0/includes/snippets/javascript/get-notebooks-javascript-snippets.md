---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 79a4156218525670c734292e3e89ca3f2950b83027e284a0c546f57ff73c02df
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278517"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let notebooks = await client.api('/me/onenote/notebooks')
    .get();

```