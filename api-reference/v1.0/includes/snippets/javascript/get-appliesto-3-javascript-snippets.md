---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 549ccf432f34445a516bfdca64677b98cc461bffa847a5a19a758e90e86ca094
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56904063"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let appliesTo = await client.api('/policies/tokenIssuancePolicies/{id}/appliesTo')
    .get();

```