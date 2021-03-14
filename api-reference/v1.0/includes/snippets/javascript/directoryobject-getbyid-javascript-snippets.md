---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dfaf3ca0eb54b9bd20a1df59b00287956b5f3916
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50798996"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
    ids: ['84b80893874940a3-97b7-68513b600544','5d6059b6368d-45f8-91e18e07d485f1d0'],
    types: ['user']
};

await client.api('/directoryObjects/getByIds')
    .post(directoryObject);

```