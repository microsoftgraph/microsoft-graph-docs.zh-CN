---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0e495d300b544983483b09e6dc274713a828e6e3
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666467"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let childFolders = await client.api('/me/mailFolders/{id}/childFolders?includeHiddenFolders=true')
    .get();

```