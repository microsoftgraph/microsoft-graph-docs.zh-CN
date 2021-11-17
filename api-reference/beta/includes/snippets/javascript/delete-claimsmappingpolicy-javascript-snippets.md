---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 77b984527660a62772569b06676664883198734872492ff32d56b25b55a56168
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274418"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/policies/claimsMappingPolicies/{id}')
    .version('beta')
    .delete();

```