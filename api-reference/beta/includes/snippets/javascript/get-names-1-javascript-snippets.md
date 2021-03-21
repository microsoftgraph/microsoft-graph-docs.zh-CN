---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7ac24e9c0e76ac104478d7898129dd7196af7c23
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50957202"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let names = await client.api('/me/profile/names')
    .version('beta')
    .get();

```