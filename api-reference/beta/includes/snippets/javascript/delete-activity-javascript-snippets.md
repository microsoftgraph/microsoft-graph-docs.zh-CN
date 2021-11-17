---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 875892db94b31aefb3f991befcde7abf5352a02369e6cd97e1c2bf0a1acd775f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220608"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/activities/13881113971988980728/')
    .version('beta')
    .delete();

```