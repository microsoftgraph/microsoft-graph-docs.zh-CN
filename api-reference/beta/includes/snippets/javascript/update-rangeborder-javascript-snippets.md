---
description: 自动生成的文件。 不修改
ms.openlocfilehash: efe5ed145f710788a949eff0b9e1d463b38530d1
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636693"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookRangeBorder = {
  color: "color-value",
  style: "style-value",
  sideIndex: "sideIndex-value",
  weight: "weight-value"
};

let res = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/format/borders/{sideIndex}')
    .version('beta')
    .update(workbookRangeBorder);

```