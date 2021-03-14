---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 14596339fb399db7ac76c629c8c2881411ca47e4
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50806115"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookApplication = await client.api('/me/drive/items/{id}/workbook/application')
    .get();

```