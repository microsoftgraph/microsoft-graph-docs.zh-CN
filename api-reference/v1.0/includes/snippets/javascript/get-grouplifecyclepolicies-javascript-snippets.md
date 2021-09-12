---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 590003b85f79196788d489691791952bbd3930985e4ff0f50dbdc2f721c3aec2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333782"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let groupLifecyclePolicies = await client.api('/groups/{id}/groupLifecyclePolicies')
    .get();

```