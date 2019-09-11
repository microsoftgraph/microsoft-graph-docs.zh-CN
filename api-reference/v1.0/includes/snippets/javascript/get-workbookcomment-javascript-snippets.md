---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b2b1cacc6d897e4b97e1a495a6ead644a06b2ecd
ms.sourcegitcommit: d8a58221ed1f2b7b7073fd621da4737e11ba53c5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/11/2019
ms.locfileid: "36839142"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/drive/root/workbook/comments/{id}')
    .get();

```