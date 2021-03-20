---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8fd569a55ee88abca1aff89a7e8f3adf6386b6ed
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50951368"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/education/schools/10001/classes/11001')
    .version('beta')
    .delete();

```