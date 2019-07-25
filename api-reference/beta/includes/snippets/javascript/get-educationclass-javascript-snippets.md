---
description: 自动生成的文件。 不修改
ms.openlocfilehash: af98064b6d8d0b45bb435863beafff942ac52716
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35712703"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/classes/11023')
    .version('beta')
    .get();

```