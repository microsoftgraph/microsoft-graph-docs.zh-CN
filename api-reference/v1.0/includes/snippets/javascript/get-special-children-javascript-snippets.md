---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5c3ca3674ec63a0ec49bcbbd96aa8da538e737e92341c3b3c017da9da8f30de0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333807"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let children = await client.api('/me/drive/special/{special-folder-name}/children')
    .get();

```