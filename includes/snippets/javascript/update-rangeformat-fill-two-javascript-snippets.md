---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4de240ee3e1a3e6b002231a89348efe27db6ebcfcc6c1716a8f79a7a3a1b6202
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54237725"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookRangeFill = {
  color: "#00FF00"
};

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$B$1')/format/fill')
    .update(workbookRangeFill);

```