---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cca2408089c6f1c9988e8706ce3ce46de1a8335e5c191f31c2c8eacec28e498f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278780"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let featureRolloutPolicy = await client.api('/policies/featureRolloutPolicies/df85e4d9-e8c4-4033-a41c-73419a95c29c')
    .version('beta')
    .expand('appliesTo')
    .get();

```