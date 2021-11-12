---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 977e364e1a41c2b6c38fd88b4efb496ea4dc013e73b9c90a8c0d27286c4fb4ac
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274359"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookNamedItem = await client.api('/me/drive/items/{id}/workbook/names/{name}')
    .version('beta')
    .get();

```