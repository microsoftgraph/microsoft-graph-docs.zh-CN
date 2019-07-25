---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c3207cc4709ebc0c17ad8d003ab205c8486df1a8
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35705708"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/classes/11021/assignments/19002/resources/22002')
    .version('beta')
    .delete();

```