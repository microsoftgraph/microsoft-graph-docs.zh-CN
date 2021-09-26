---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9b5d93427f85365abb707d720b908968857d165cdaf8ccfdc960c9cc3f3a7dfa
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273884"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let memberOf = await client.api('/groups/{id}/memberOf')
    .version('beta')
    .get();

```