---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 559344d7ebef9e7db480d8c05644d2cd1b951554
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35739982"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education')
    .get();

```