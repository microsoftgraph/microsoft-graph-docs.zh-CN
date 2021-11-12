---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1efb143a4ddb0166f929c0cc04d7f17d2f3263e3165c2c48e0ef7a4852bf63f7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161654"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookRange = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/DataBodyRange')
    .version('beta')
    .get();

```