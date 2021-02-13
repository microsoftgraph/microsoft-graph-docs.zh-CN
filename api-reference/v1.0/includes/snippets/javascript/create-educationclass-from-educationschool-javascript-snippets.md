---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e24413f1254680ce72f348d3c04fc1be56851337
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/10/2021
ms.locfileid: "50178986"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/classes/{class-id}/teachers/{teacher-id}')
    .delete();

```