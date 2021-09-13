---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 82039fbcca75844547ba9198036312911f9b2301a6e240caa88d65ae811a67b9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161322"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let stream = await client.api('/identity/b2xUserFlows/B2X_1_Partner/languages/en/defaultPages/idpselections/$value')
    .get();

```