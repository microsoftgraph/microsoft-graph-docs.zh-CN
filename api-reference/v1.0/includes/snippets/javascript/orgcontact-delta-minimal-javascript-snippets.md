---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8cefbf96a693b168b0bb6c4208abf68d39cdcacb53de96fc22b4bd50108191c6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218721"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delta = await client.api('/contacts/delta')
    .header('Prefer','return=minimal')
    .select('displayName,jobTitle,mail')
    .get();

```