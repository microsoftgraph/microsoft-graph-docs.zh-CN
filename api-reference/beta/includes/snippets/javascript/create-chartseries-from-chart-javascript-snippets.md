---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 02b7e4c7ad42736c2cbd206a9c414d253507b3afb39b1074b512fe930e554e04
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332314"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookChartSeries = {
  name: 'name-value'
};

await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series')
    .version('beta')
    .post(workbookChartSeries);

```