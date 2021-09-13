---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eee7829bf0c12040b1e6a0539d4b65d02dc64c921647fddbe2f2dbe03f7c2b73
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161961"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookRange = await client.api('/me/drive/root/workbook/worksheets/{id}/range/rowsAbove')
    .get();

```