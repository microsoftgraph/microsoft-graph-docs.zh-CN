---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 92f476e580c98f2dfc11158131da286ff821c3fcf03361b6a64bd85fd48d79cf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274376"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const permission = {
  type: 'embed'
};

await client.api('/sites/{siteId}/lists/{listId}/items/{itemId}/createLink')
    .version('beta')
    .post(permission);

```