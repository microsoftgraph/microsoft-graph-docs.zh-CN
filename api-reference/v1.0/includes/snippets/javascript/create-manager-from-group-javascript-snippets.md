---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b261ac6554656669f8dac5511a9aaf45a42892a2
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35885589"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
  @odata.id: "https://graph.microsoft.com/v1.0/users/{id}"
};

let res = await client.api('/users/{id}/manager/$ref')
    .put({directoryObject : directoryObject});

```