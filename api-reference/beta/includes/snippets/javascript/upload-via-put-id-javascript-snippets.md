---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 056f1bb68586a9b5846bf2e03b1ed68aea7419b5
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35712785"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const Stream = The contents of the file goes here.;

let res = await client.api('/me/drive/items/{item-id}/content')
    .version('beta')
    .put({Stream : Stream});

```