---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ace51b29cd55ff6ee7d157012ee4df78de43264a
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35710118"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/applicationTemplates')
    .version('beta')
    .get();

```