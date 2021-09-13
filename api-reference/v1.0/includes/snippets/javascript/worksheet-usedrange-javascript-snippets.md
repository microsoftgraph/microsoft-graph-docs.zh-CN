---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d4a98787a24b8846e68a453704904c7729bca4d52b04f7b39b144cde05c65caa
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273919"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookRange = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/usedRange')
    .get();

```