---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 43dcfaf5985c06a20e3b57bb6f1a8488835311a1fdd60bb969bf57e613350fa1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277821"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let channel = await client.api('/teams/893075dd-2487-4122-925f-022c42e20265/channels/19:561fbdbbfca848a484f0a6f00ce9dbbd@thread.tacv2')
    .version('beta')
    .get();

```