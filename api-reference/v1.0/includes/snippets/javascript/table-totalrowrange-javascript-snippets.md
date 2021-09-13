---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 27798382675586e54e0f2946e6db07761556cd9132c42cfd03198762bc30d325
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106411"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookRange = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/totalRowRange')
    .get();

```