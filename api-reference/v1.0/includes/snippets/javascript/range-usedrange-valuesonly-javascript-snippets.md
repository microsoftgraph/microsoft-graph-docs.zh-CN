---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 436e46bb26c81876cd96dec4277a7d2c008c69f00c713c83773f4a2817d12bec
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56904093"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookRange = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/usedRange(valuesOnly=true)')
    .get();

```