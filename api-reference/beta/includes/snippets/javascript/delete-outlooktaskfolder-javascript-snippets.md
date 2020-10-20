---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ac666ae15eeae2ab936cf377150710ef8e1efbe4
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48603445"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/outlook/taskFolders/AAMkADIyAAAhrbPXAAA=')
    .version('beta')
    .delete();

```