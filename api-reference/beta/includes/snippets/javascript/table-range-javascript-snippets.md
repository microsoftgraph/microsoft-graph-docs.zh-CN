---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b391ad57f59d03a54f777a4178b8d48d9f9bc00c
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43805761"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/Range')
    .version('beta')
    .get();

```