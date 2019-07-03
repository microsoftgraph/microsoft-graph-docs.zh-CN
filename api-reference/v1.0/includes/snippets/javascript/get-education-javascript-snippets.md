---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 559344d7ebef9e7db480d8c05644d2cd1b951554
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35492995"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education')
    .get();

```