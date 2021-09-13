---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1e17316ee6159984bf80a3d92dd5ef22adecdfbf9c765aacebbe845ad30f9b9a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278601"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookChartSeries = {
  index: 2
};

await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series/itemAt')
    .post(workbookChartSeries);

```