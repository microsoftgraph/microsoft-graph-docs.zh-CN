---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 12c1a1901f1446a1626db9af7278b25866bd1369de776ea88b0775d8f0fcebb4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105669"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let names = await client.api('/me/drive/items/{id}/workbook/names')
    .get();

```