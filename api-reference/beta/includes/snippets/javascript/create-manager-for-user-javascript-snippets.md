---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7179a28ec92b5ae59f9542444e30f11577b37b2f371d9e9f770915898d8e8a7a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163334"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
  '@odata.id': 'https://graph.microsoft.com/v1.0/users/{id}'
};

await client.api('/users/{id}/manager/$ref')
    .put(directoryObject);

```