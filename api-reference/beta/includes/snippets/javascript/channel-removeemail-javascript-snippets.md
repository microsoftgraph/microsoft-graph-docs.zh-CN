---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 47aaef8fda1f14e1fc890906e494eede8f5e6f018df63cedd1d8834f70dcda11
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902854"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/teams/893075dd-2487-4122-925f-022c42e20265/channels/19:561fbdbbfca848a484f0a6f00ce9dbbd@thread.tacv2/removeEmail')
    .version('beta')
    .post();

```