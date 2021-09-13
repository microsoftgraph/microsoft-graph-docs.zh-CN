---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7a1027277fff945117b27a87238e47827e190012f09ef58bd14501fbda19b4d0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220725"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let overridesPages = await client.api('/identity/b2xUserFlows/B2X_1_Partner/languages/en/overridesPages')
    .get();

```