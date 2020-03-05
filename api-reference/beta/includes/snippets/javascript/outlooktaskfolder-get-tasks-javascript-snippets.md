---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 415130b42816d8c865d2c07d0d2f5dae629b13e0
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "37637504"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/outlook/taskFolders/AAMkADIyAAAhrbPWAAA=/tasks')
    .version('beta')
    .get();

```