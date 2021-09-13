---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 87882667c2a75a6bc1dc46cf9d94e9723c953fecaba1370ebdffb58d9169a000
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104922"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let tokenIssuancePolicy = await client.api('/policies/tokenIssuancepolicies/{id}')
    .get();

```