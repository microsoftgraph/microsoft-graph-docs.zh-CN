---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bc83b943cf628120b7121cc7d56c53e099ebf92ed5d0dc8a70fdf470a6820b06
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378693"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let installedApps = await client.api('/teams/6903fa93-605b-43ef-920e-77c4729f8258/installedApps')
    .expand('teamsAppDefinition')
    .get();

```