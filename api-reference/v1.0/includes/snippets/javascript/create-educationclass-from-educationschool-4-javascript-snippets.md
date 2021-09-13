---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cfbd59c20f9bea641a77c3f14f457b6ff28ba585fc7a62550b78504b44fe5d55
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902280"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/education/schools/{school-id}/users/{user-id}')
    .delete();

```