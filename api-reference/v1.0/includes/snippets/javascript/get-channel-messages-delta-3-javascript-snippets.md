---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4f62860c7bb286b93a54d8f2f333e779cb5ebc05
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48905023"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teams/{id}/channels/{id}/messages/delta')
    .skiptoken('c3RhcnRUaW1lPTE1NTEyODcyMzY2NzgmcGFnZVNpemU9MjA=')
    .get();

```