---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2699e253f25353463eb1152189b8b537928ddd6862fada207aaa5e1614b4058c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57334069"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/servicePrincipals/{id}/claimsMappingPolicies/{id}/$ref')
    .delete();

```