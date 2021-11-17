---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b1e8bc3be517e05df74c5386f2cb636f04ce32c2f41cd4cdd9cf277cc9882ef1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220250"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let room = await client.api('/places/microsoft.graph.room')
    .version('beta')
    .get();

```