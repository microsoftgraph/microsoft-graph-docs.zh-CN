---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 41fcc3d4cd2c7bd233c5f7d8fe84f3fa7b408884039fc8db9abf4206dff59474
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409650"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let rows = await client.api('/me/drive/root/workbook/worksheets/{id}/range(address='A1:Z10')/visibleView/rows')
    .get();

```