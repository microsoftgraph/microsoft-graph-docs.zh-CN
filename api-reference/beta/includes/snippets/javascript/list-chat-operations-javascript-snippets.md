---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a8a1b4b57884e33bbbfb88831b44a8f70bb8f798b72779c490999111d84b9640
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106941"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let operations = await client.api('/chats/19:c253a29b5f694b55a6baad8e83510af7@thread.v2/operations')
    .version('beta')
    .get();

```