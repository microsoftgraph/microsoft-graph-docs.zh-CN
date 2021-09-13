---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 47b88b234cc8da9c45d368e6f5bc1949be132bfb765910973d1cea1fa8b5c9a2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221210"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let lists = await client.api('/me/todo/lists')
    .version('beta')
    .get();

```