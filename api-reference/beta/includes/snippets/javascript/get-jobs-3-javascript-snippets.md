---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 58a95f0c4b27663cb3fe1e89de665a7a7eca4cb89435af3c376568c6c4d3173d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104480"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let jobs = await client.api('/servicePrincipals/{id}/synchronization/jobs/')
    .version('beta')
    .get();

```