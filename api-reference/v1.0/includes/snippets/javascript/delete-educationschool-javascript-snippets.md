---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 71bff0193aa064d77d8cc529a60e7e2e4b70e68eaee9475aec046a653082d282
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274076"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/education/schools/{school-id}')
    .delete();

```