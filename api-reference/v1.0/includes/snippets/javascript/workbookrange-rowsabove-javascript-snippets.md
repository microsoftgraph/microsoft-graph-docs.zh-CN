---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ccecc07bf6ab25f629705ec84be886a7b88116c452d9b03c12352c284de7cad1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161964"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookRange = await client.api('/me/drive/root/workbook/worksheets/{id}/range/rowsAbove(count=2)')
    .get();

```