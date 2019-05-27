---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 579d70e82cf18190a8e77a39a900b0f152c4e410
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34443584"
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