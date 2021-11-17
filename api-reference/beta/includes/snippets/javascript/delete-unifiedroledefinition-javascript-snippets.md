---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fb9da13eda7e5aabb28e3d1e515df9e3aa0a0001b524f1408a25e50ee2f5a683
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278883"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/roleManagement/directory/roleDefinitions/f189965f-f560-4c59-9101-933d4c87a91a')
    .version('beta')
    .delete();

```