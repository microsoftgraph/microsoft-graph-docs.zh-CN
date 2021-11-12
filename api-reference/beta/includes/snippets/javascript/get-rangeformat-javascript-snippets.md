---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6546511cd2997fac6e1c31350b85e3b0845a9d8db21f3cd95fb80596cf4f6e3f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278156"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookRangeFormat = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/format')
    .version('beta')
    .get();

```