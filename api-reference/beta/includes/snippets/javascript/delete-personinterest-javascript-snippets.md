---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7a002512c4495e1e10b9fda3900fa0897df10b44
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "37998130"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/profile/interests/{id}')
    .version('beta')
    .delete();

```