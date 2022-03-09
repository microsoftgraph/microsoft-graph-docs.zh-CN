---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1b0d07c63fbaf87c8aef218c1e7a7853e311342fb9e0f4832bfd0e39438c87a3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220292"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/education/schools/10001/users/13006')
    .version('beta')
    .delete();

```