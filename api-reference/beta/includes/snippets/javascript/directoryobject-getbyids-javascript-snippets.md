---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d034a18a0e781f467579c72977a665005a11c384a638b31a5faa643c23fe830d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57328806"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
    ids: ['84b80893-8749-40a3-97b7-68513b600544','5d6059b6-368d-45f8-91e1-8e07d485f1d0'],
    types: ['user']
};

await client.api('/directoryObjects/getByIds')
    .version('beta')
    .post(directoryObject);

```