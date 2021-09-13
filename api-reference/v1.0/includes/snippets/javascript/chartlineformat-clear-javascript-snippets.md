---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bdcbd1e71a2be8e5dbf7f484a26995cb91182508c36fc799c895a29c01b510b8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274088"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis/format/line/clear')
    .post();

```