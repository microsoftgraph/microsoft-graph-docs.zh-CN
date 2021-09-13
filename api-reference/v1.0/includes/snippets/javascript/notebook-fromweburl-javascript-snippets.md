---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 030342aad511f404f66ccb660dbcc1546caf26513b06886382af692d940826b2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104570"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const copyNotebookModel = {webUrl: 'webUrl value'};

await client.api('/me/onenote/notebooks/GetNotebookFromWebUrl')
    .post(copyNotebookModel);

```