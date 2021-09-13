---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5998dbfd3387f3703d7b1e39ed3094709db3b63c8daa003dbfa36f90e2ce2d32
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409457"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookApplication = await client.api('/me/drive/items/{id}/workbook/application')
    .get();

```