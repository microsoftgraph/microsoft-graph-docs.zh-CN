---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 10bd436aca58c87a62e2d0366dfb4e9815c756acba5a0dd43b20e478d5fa0a75
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161767"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delta = await client.api('/users/delta')
    .get();

```