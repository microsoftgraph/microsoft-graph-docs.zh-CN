---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 258bfa17fc77231db27bcf4615961ef1791690f0df501a7115bf4ba96968df3c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57164222"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookRange = await client.api('/me/drive/root/workbook/worksheets/{id}/range/rowsBelow')
    .get();

```