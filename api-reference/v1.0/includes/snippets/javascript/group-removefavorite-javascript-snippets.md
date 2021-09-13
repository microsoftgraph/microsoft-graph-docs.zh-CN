---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f8f7205432a61aa71f0f36fab224e8b441dbc9495ebeb017c136e1ab5f62c8e1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220410"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/groups/{id}/removeFavorite')
    .post();

```