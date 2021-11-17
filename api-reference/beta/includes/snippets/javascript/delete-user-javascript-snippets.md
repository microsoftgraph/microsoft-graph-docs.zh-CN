---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: af6f5b525f11689e8333cdb277cb81c3e5e06dd72d3607e4fb0cb8ba618f57d7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163912"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/users/ba9a3254-9f18-4209-aeb3-9e42a35b5be4')
    .version('beta')
    .delete();

```