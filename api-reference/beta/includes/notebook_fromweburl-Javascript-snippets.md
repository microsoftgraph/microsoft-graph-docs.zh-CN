---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 2692af271f11f35f251c11a7a437439d4d57a712
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34443773"
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