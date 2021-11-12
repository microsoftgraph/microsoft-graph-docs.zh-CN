---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0ab2fd1698e5ea924fd4a26ea76b05adb2808a0a0454350081a79e2e0cd2dc2e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57164210"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let conversationThread = await client.api('/groups/{id}/threads/{id}')
    .version('beta')
    .get();

```