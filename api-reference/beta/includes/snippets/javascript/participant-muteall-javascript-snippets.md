---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 579d70e82cf18190a8e77a39a900b0f152c4e410
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35521072"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const CommsOperation = {
  participants: [
    ""
  ],
  clientContext: "clientContext-value"
};

let res = await client.api('/app/calls/{id}/participants/muteAll')
    .version('beta')
    .post(CommsOperation);

```