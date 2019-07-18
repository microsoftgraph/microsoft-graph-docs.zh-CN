---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9f765955a4fd0dac2977a816e8aa87fbb9378c4d
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35707649"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/chats/{id}/messages/{id}/replies')
    .version('beta')
    .get();

```