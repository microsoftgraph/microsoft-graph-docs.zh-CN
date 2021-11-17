---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0c3a557fd49a0b4eb1140bb59fbb8603646a1e7add3aa2d23c7e092c76dfd012
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161273"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let operations = await client.api('/compliance/ediscovery/cases/061b9a92-8926-4bd9-b41d-abf35edc7583/operations')
    .version('beta')
    .get();

```