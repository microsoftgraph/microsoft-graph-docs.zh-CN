---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: adf6d420d7dd881ae4dc12229aa8d52dc84a5341f6f8068580f7b578ebd7b379
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279575"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookRange = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/EntireRow')
    .version('beta')
    .get();

```