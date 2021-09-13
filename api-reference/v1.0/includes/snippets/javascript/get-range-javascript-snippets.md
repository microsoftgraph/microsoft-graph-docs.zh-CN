---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7bfaa1dd43544b78a2e4e5fe9cf6123684466b4e965d9577eafff0dc470e83ed
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333909"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookRange = await client.api('/me/drive/items/{id}/workbook/names/{name}/range')
    .get();

```