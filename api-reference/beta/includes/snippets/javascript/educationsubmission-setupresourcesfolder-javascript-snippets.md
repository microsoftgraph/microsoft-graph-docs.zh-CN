---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 20fe5c924e8df17d5af5501ea50f123d096fdcb2
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52664771"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/education/classes/11012/assignments/19002/submissions/20302/setUpResourcesFolder')
    .version('beta')
    .post();

```