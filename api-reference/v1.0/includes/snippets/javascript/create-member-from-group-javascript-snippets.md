---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 42ec5fbf8cf40ab234981f25bfe23347f79d1cdb
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35890077"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
  @odata.id: "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
};

let res = await client.api('/groups/{id}/members/$ref')
    .post({directoryObject : directoryObject});

```