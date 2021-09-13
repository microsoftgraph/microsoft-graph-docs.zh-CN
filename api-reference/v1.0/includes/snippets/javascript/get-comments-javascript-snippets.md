---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 470c11486cdd1571018e78b1db9efe4c753deaf54a13a2ec3629f19024aafd6a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409298"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let comments = await client.api('/drive/items/{id}/workbook/comments')
    .get();

```