---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 5e013d191f751ae21c4f4f9fbfc50312c52ef68c
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35738695"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/contacts')
    .get();

```