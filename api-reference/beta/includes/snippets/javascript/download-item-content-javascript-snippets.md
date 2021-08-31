---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dda7ce7aae1583d8e00a42a5cb778c376b1d39c3069dc8075d1c7ec08301dd3b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105165"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let stream = await client.api('/me/drive/items/{item-id}/content')
    .version('beta')
    .get();

```