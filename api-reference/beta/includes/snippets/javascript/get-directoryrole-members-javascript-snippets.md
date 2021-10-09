---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6fb0dc55fa1b54190f5f7e56760c633cb8a4f77acdf7422a65206eb9666892be
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221247"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let members = await client.api('/directoryRoles/23f3b4b4-8a29-4420-8052-e4950273bbda/members')
    .version('beta')
    .get();

```