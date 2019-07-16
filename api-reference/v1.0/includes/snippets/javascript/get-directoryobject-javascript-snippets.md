---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 0272628e74cc997702120b64da4627da2e4e4ee1
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35737903"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/directoryObjects/{id}')
    .get();

```