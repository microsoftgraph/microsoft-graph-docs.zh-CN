---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1683c108e1a181f151c44584a00b33f1de389d01b41780b572eef72a21f0c8f8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56904202"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookRange = await client.api('/drive/root/workbook/worksheets/{id}/range/columnsAfter(count=2)')
    .version('beta')
    .get();

```