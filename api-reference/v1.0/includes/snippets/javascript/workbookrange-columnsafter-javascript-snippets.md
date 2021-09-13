---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: abb453696bbb871a10de2e85a73a4f478b2d25057280ed16dcf502ded53683f9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279295"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookRange = await client.api('/me/drive/root/workbook/worksheets/{id}/range/columnsAfter(count=2)')
    .get();

```