---
description: 自动生成的文件。 不修改
ms.openlocfilehash: bf56af01bb6c724ad6c8c7f1814e1d5b6571b7b1
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35706739"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
    ids:["84b80893-8749-40a3-97b7-68513b600544","5d6059b6-368d-45f8-91e1-8e07d485f1d0"],
    types:["user"]
};

let res = await client.api('/directoryObjects/getByIds')
    .version('beta')
    .post(directoryObject);

```