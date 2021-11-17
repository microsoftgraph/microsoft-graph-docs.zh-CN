---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 22ea905f0a54b97d2e52c8007020c468aaa135605f56a2accf106e63813153d5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105690"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/revokeSignInSessions')
    .version('beta')
    .post();

```