---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dd8359d1186487b2e0865cd5852323cbf9193e552f210456eea07c6a46b518e4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158728"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let calendar = await client.api('/me/calendar')
    .get();

```