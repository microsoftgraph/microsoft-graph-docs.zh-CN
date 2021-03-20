---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7ca4a43e942397849a49bea7846fc9a164c02944
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50946745"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
  '@odata.id': 'https://graph.microsoft.com/beta/directoryObjects/{id}'
};

await client.api('/devices/{id}/registeredOwners/$ref')
    .version('beta')
    .post(directoryObject);

```