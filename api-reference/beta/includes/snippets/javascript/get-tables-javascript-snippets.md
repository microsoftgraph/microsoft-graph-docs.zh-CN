---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f7c8e6748e86998b8ffc7c5cb21b3db22fa0b896
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2021
ms.locfileid: "49946200"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/tables')
    .version('beta')
    .get();

```