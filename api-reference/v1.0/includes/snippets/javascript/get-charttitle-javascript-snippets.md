---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a3d5d5b415230616853874886bb4163b6789b5720190f87e59c467646fe7bdf8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221020"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookChartTitle = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/title')
    .get();

```