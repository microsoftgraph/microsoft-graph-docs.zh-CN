---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 963110aa3067c5f97fc0c7a477ce944a306c55cc6df36fb58bb26cbce9a22571
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104296"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/drive/items/{id}/workbook/names/{name}/range/unmerge')
    .post();

```