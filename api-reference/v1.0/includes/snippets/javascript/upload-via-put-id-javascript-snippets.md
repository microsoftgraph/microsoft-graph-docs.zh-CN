---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0bd91c7741e4e69565e0a4b080e02140c6e1ef5a9709275be581b20ddfa3d115
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57334124"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const stream = The contents of the file goes here.;

await client.api('/me/drive/items/{item-id}/content')
    .put(stream);

```