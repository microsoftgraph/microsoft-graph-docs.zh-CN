---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4ef1a3d5c83bfeafab9c53cbcea1066d3665a52a
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65212202"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let documentSetVersions = await client.api('/sites/root/lists/Documents/items/1/documentSetVersions')
    .version('beta')
    .get();

```