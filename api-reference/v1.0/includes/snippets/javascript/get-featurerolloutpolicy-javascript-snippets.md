---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 244e1a7fae391390b3deb6883ea3ce7c25525a893fa7ec0cbaa928f9b67bd1e9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278839"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let featureRolloutPolicy = await client.api('/policies/featureRolloutPolicies/df85e4d9-e8c4-4033-a41c-73419a95c29c')
    .get();

```