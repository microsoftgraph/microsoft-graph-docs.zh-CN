---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8c77c3b25ac4f9ae1c208e2f2c94ac24fd04d92f5134fd0d3a59a644f3f2e096
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105737"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let supportedTimeZones = await client.api('/me/outlook/supportedTimeZones')
    .version('beta')
    .get();

```