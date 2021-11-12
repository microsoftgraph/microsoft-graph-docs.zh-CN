---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 196eac1c20df045977bae0767008dce8a776b7f4134193c53f46277ba1e04768
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220534"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let connectors = await client.api('/onPremisesPublishingProfiles/applicationProxy/connectors')
    .version('beta')
    .get();

```