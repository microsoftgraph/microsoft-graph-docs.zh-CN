---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 282e82bdcf3838b0be1efe35fa2b89da9fffb81cec295fb46cd77cbbf644559d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163596"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let user = await client.api('/me')
    .version('beta')
    .get();

```