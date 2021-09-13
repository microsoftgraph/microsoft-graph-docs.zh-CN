---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 709108206e15d26075ec9751d4cfe83b44f480ae3280d4f0d02edc33e7f531f0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104964"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookNamedItem = await client.api('/me/drive/items/{id}/workbook/names/{name}')
    .get();

```