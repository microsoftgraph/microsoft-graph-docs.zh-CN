---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 041c78f529cbd674ac3f0da5f8021ce15e27a73919679a36c27de0d3a78dfaea
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215633"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let appliesTo = await client.api('/policies/homeRealmDiscoveryPolicies/{id}/appliesTo')
    .version('beta')
    .get();

```