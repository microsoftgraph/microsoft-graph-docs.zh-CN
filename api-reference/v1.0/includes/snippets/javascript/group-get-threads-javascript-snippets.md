---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4cdc160a23ae5431aee16fa7ac7c5ab8566a3557
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50801906"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let threads = await client.api('/groups/{id}/threads')
    .get();

```