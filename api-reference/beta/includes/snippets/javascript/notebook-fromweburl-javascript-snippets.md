---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 2692af271f11f35f251c11a7a437439d4d57a712
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35521089"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const CopyNotebookModel = {webUrl:"webUrl value"};

let res = await client.api('/me/onenote/notebooks/GetNotebookFromWebUrl')
    .version('beta')
    .post(CopyNotebookModel);

```