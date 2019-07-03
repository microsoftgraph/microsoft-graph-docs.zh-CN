---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c93c8acf64270cf6688191b77400f4091da6da54
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35493406"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const CopyNotebookModel = {webUrl:"webUrl value"};

let res = await client.api('/me/onenote/notebooks/GetNotebookFromWebUrl')
    .post(CopyNotebookModel);

```