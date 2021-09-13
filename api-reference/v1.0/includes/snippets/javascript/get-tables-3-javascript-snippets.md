---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b978c65656bac65521eb3cb372c5fb4e16af3ad17867ba217d60b564e658d369
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218623"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let tables = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/tables')
    .get();

```