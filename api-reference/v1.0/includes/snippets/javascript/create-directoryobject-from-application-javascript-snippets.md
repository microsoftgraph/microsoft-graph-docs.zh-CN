---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2cca0f5e6fe2b048689dea399b744d69d9f988914eecc3570ccf9054d137ec5d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57334008"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
    '@odata.id': 'https://graph.microsoft.com/v1.0/directoryObjects/{id}'
};

await client.api('/applications/{id}/owners/$ref')
    .post(directoryObject);

```