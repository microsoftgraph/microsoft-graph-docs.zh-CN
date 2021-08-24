---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9ee9b17fb06f798d73932718b7a9fb24e4c3c588721704685b42a3241540eb5e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332589"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delta = await client.api('/groups/delta')
    .get();

```