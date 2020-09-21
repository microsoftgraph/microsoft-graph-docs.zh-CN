---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9a5cb493fa39e4bfc222441babf468a9601e0cc1
ms.sourcegitcommit: ef47b165f7a140cfc0309a275cb8722dd265660d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2020
ms.locfileid: "46872582"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/todo/lists/AAMkADIyAAAhrbPXAAA=')
    .version('beta')
    .delete();

```