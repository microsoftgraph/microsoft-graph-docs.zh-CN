---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 699d450a118bfb5fa4dd09982c92bcb1e4f966f659952256eb312e5dcf169e68
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57107148"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delta = await client.api('/directoryRoles/delta')
    .get();

```