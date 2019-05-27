---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 6559999e0a6c3f4f0bbb90efc77030e67993454f
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34460627"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const outlookTaskFolder = {
  name: "Charity work"
};

let res = await client.api('/me/outlook/taskFolders/AAMkADIyAAAhrbPWAAA=')
    .version('beta')
    .update({outlookTaskFolder : outlookTaskFolder});

```