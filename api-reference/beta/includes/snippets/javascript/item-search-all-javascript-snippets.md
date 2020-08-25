---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fe4fe0828227825b81c636d04de7b918c90e1047
ms.sourcegitcommit: ef47b165f7a140cfc0309a275cb8722dd265660d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2020
ms.locfileid: "46873874"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/search(q='Contoso Project')')
    .version('beta')
    .get();

```