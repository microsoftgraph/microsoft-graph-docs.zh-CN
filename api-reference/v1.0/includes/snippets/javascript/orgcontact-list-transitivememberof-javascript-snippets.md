---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ff224aca4eb6f6a8a4fd766f0bdc911ed06b27f4f763357710d9a87d6d215ae1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378423"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let transitiveMemberOf = await client.api('/contacts/{id}/transitiveMemberOf')
    .get();

```