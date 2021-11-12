---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5803ec4fc510f04c25da62be117ddbbad04876ee4af9395973d64592446b0cab
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158313"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookChartDataLabels = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/datalabels')
    .version('beta')
    .get();

```