---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b6be16b332f3985f4c0f7b405b476a034ecdd79e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50781404"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let getRecentNotebooks = await client.api('/me/onenote/notebooks/getRecentNotebooks(includePersonalNotebooks=true)')
    .get();

```