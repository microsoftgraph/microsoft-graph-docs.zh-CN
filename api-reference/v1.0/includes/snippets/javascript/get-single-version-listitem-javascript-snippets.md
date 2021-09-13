---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4d97d6b31c473ba50c196789289d4b0bfc56079a14b36554383c1e8367510344
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409030"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let listItemVersion = await client.api('/sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}?expand=fields')
    .get();

```