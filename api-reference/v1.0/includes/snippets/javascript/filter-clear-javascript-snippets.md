---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 81ac275805919fbfc7a50286a3fcf40caea21768bf6bf0a778036df51df4e8e3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278838"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/filter/clear')
    .post();

```