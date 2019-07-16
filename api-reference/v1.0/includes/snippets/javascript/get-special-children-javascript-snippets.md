---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 57473cbb142913cac15f7cc69b15304a822415f3
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35736376"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/special/{special-folder-name}/children')
    .get();

```