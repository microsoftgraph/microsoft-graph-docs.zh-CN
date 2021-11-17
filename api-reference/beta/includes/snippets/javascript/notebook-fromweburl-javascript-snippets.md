---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b396dafcbd07bbba3abcd0c9ec01dac30637e9350bfc2c7cf762fd5e675b8bd1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162879"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const copyNotebookModel = {webUrl: 'webUrl value'};

await client.api('/me/onenote/notebooks/GetNotebookFromWebUrl')
    .version('beta')
    .post(copyNotebookModel);

```