---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 40b1fb66213fc4d4bfa02bdc3c9cddc064a01219
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50957676"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
  directoryObject: {
  }
};

await client.api('/contacts/{id}/memberOf')
    .version('beta')
    .post(directoryObject);

```