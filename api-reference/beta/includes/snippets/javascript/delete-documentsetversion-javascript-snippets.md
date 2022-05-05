---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e31fce9edce682cfeda6640bbf44f73139550b9a
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65208692"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/sites/root/lists/Documents/items/2/documentSetVersions/1')
    .version('beta')
    .delete();

```