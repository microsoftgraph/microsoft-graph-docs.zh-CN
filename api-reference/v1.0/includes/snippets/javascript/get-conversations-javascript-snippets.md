---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 98323016d2dd88113b9389ebfc802bbbac3270ba546dd15ef8632a1cc0325f2e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278217"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let conversations = await client.api('/groups/{id}/conversations')
    .get();

```