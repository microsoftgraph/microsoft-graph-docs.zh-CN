---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b711f61baefc94a59a130e487fffe364c7250fd3
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48614030"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const exportPersonalData = {
  storageLocation: "storageLocation-value"
};

let res = await client.api('/users/{id}/exportPersonalData')
    .version('beta')
    .post(exportPersonalData);

```