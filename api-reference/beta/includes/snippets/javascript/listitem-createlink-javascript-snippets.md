---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 46eeda1d9b28b2b43f58b90575c62d6ffd63b746
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52992381"
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