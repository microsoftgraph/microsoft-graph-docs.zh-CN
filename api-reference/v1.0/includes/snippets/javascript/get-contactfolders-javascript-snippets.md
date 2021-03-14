---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3026ea677f20c5858e548241b2a55dbcb179795f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50790272"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let contactFolders = await client.api('/me/contactFolders')
    .get();

```