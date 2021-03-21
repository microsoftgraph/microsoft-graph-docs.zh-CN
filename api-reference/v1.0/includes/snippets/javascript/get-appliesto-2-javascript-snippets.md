---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4f4e2b6b107a2677d3b9da660266c15a3c89b13f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50959810"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let appliesTo = await client.api('/policies/homeRealmDiscoveryPolicies/{id}/appliesTo')
    .get();

```