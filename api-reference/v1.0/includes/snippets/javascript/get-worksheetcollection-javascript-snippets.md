---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 179e8e0034f48530e1728c5bd3ddfcabe4bffed7a94c8eb86640a905de6f9ccb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106963"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let worksheets = await client.api('/me/drive/items/{id}/workbook/worksheets')
    .get();

```