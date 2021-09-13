---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 20674b0c689e80c63b3dac8c56ca31ea88c29e02b3770588a283815d7f54fae8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105333"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/drive/items/{id}/workbook/names/{name}/range/format/autofitColumns')
    .post();

```