---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ebdd6cb368708201b5a17530a05d35fb331d13445348fad6410f5c8edb81c6ae
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220252"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let roomlist = await client.api('/places/microsoft.graph.roomlist')
    .version('beta')
    .get();

```