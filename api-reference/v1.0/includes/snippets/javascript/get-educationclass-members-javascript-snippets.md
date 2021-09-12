---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e52bdafef0e912377402c43a84cffa7b44d4bf8ca6986a0ccf8f6ddfce354060
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378323"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let members = await client.api('/education/classes/{class-id}/members')
    .get();

```