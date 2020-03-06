---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4fc664182a69dbe49a8e3f69322b3e276c9347ad
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636866"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
  @odata.id: "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
};

let res = await client.api('/directoryRoles/{id}/members/$ref')
    .post(directoryObject);

```