---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4aa38c228ea6932deb51c115df49cdf8efdc7350
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50806498"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let stream = await client.api('/me/messages/4aade2547798441eab5188a7a2436bc1/$value')
    .version('beta')
    .get();

```