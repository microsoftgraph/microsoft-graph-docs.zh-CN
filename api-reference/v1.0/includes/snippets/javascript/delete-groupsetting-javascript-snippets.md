---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3735de0ba64d32f08697e28449d379c2543b3c20480639b68da1fa1135f92db9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279186"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/groupSettings/{id}')
    .delete();

```