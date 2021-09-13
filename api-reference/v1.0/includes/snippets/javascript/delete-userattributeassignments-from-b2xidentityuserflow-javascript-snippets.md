---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7b0292e81be7e9b139c92015e8f6afd47d9432f41f2642e6e8d96a28bca3130f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409523"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/identity/b2xUserFlows/B2X_1_Partner/userAttributeAssignments/City')
    .version('beta')
    .delete();

```