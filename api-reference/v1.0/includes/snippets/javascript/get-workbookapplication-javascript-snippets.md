---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7ea4e54206c826710d9bfe640a0e0d848bd7627d
ms.sourcegitcommit: fa08172601324fc01b090f8135fba4600bd1a9f8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/13/2019
ms.locfileid: "38302316"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/application')
    .get();

```