---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8e5b285ee1f14d2fb5230e4d2e33f2c23147a5ed21f4cccc296e9434c5627a1e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903500"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/profile/websites/{id}')
    .version('beta')
    .delete();

```