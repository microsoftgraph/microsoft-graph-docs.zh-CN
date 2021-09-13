---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8c645760f83241787a3c12601e214d10f9bac73838fcee34f1ead3c0d2bf822b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163328"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookComment = await client.api('/drive/items/{id}/workbook/comments/{id}')
    .version('beta')
    .get();

```