---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c5b39a445e1d621532d67a5d5784514fd9e87b441b005745e12251b5b626317a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163578"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workforceIntegrations = await client.api('/teamwork/workforceIntegrations')
    .version('beta')
    .get();

```