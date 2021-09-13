---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ec39443db913330f7b8be03a386eea8c7a600dec122fafc33c5c3df0d0f98a33
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409343"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/connections/contosohr/items/TSP228082938')
    .delete();

```