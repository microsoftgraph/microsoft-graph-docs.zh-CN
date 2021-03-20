---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 272810aded1b8208ce652f5bd6a8e6c5586db80d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50953255"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let taskFolders = await client.api('/me/outlook/taskGroups/AAMkADIyAAAhrbe-AAA=/taskFolders')
    .version('beta')
    .get();

```