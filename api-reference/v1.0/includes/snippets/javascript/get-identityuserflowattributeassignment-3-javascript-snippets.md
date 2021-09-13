---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 559161968afa93f20a4861b928575d828b8198c5a277f5063a0017d4f632736e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378751"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let identityUserFlowAttributeAssignment = await client.api('/identity/b2xUserFlows/B2X_1_Partner/userAttributeAssignments/City')
    .get();

```