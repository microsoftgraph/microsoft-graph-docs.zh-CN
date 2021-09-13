---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9b9ef115b4d28b2450ec83491ff869e661ed2e2fc2fbb8c4791adbb5ab003ae4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57328902"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookChartLegend = {
  visible: true,
  position: 'position-value',
  overlay: true
};

await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/legend')
    .update(workbookChartLegend);

```