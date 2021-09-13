---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0bcde3aa713286bc40c9040626bcffdc73b6d0fc05fa9366c9e7047fbe0c11d3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219985"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookRange = await client.api('/me/drive/root/workbook/worksheets/{id}/range/columnsBefore(count=2)')
    .get();

```