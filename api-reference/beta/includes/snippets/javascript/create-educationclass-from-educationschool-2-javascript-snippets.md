---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1c51c3bbfecc65987b683fb28c2c3fb1fc7af94f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50951627"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/education/classes/{id}/teachers/14012')
    .version('beta')
    .delete();

```