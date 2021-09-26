---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8d6eefece9a37bda9e1967202d73dcde8e43868fd4758fb7e1e02ddc419babd3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903831"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/teams/893075dd-2487-4122-925f-022c42e20265/channels/19:561fbdbbfca848a484f0a6f00ce9dbbd@thread.tacv2/provisionEmail')
    .version('beta')
    .post();

```