---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4b1de2241eb8b87c90a3aac8c610d193e4ccecdcd4033dd80f83ebe7041ebc42
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104621"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookChartGridlines = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis/minorGridlines')
    .get();

```