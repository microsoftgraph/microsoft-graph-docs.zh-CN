---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 42922a7ba374f216700d2b35e673c5c78ffc8bf0c25ab213070c5965c2407499
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220122"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let installedApps = await client.api('/users/5b649834-7412-4cce-9e69-176e95a394f5/teamwork/installedApps')
    .expand('teamsAppDefinition')
    .get();

```