---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a071be6a648c68e7917c737dc7677f9e6c7a312a
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/11/2020
ms.locfileid: "49659079"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const siteSource = {
    site@odata.bind: "https://graph.microsoft.com/v1.0/sites/{siteId}"
};

let res = await client.api('/compliance/ediscovery/cases/4c8f8f70-7785-4bd4-b296-c98376a2c5e1/custodians/2192ca408ea2410eba3bec8ae873be6b/siteSources')
    .version('beta')
    .post(siteSource);

```