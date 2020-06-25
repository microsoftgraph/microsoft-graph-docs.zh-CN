---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5a4ad16ce9acbf34aa7f9c226e1c3a10aa784cb4
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863290"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/policies/claimsMappingPolicies')
    .get();

```