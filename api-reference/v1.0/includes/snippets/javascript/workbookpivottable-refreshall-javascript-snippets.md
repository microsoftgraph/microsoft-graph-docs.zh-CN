---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2970c016ee0bbf8b16a8798387c773b2e17006abcb1283fe56cb5cf42e426f85
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158677"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/drive/root/workbook/worksheets/{id}/pivotTables/refreshAll')
    .post();

```