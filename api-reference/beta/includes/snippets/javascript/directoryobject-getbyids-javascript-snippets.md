---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 129356f754d5c0028ea1f7b6c8c07868eb053b6e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50778965"
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