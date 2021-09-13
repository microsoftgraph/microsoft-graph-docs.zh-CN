---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 19c718068a7285e605b568b5facbb5ab092e00eeb5719c80c040a6b366bbfd9c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161601"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let tokenIssuancePolicies = await client.api('/policies/tokenIssuancePolicies')
    .get();

```