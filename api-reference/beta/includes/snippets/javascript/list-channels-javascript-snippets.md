---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f547c69e890ca74a18abdae16eeb8ba54b07f072
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50780335"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let channels = await client.api('/teams/{id}/channels')
    .version('beta')
    .get();

```