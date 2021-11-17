---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0205086280c656596144046ec2bd1ccf17c7d35daeeaca0f6e094aa792deb223
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57164013"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let claimsMappingPolicy = await client.api('/policies/claimsMappingPolicies/{id}')
    .version('beta')
    .get();

```