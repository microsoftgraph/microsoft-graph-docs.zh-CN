---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b5056a28c32d5202cc0da86d5d828afd27693f7b
ms.sourcegitcommit: 01f73b4dce6f885da18d62fe800b387c286c7a8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/09/2020
ms.locfileid: "47413328"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
  @odata.id: "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
};

let res = await client.api('/groups/{group-id}/members/$ref')
    .post(directoryObject);

```