---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4cb6d560f2629876c4fe0c1bcd746b5d826e9349b3037f93b26494179987f811
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162329"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookRange = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/totalRowRange')
    .get();

```