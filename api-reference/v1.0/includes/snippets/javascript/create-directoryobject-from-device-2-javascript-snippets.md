---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: db183417f6610020af8ad865d76a45ba9b29ecd8a50c2722198abe84a626ecc2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332441"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
  '@odata.id': 'https://graph.microsoft.com/v1.0/directoryObjects/{id}'
};

await client.api('/devices/{id}/registeredUsers/$ref')
    .post(directoryObject);

```