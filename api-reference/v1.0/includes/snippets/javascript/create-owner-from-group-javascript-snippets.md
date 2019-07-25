---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8fc589501d8f77ca24b728a3e30cd55a0698f0f6
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35884750"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
  @odata.id: "https://graph.microsoft.com/v1.0/users/{id}"
};

let res = await client.api('/groups/{id}/owners/$ref')
    .post({directoryObject : directoryObject});

```