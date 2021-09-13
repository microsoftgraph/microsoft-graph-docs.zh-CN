---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 87b1a807685b38e645ebffdccd124376ec8ea976b7d536790dc15d5218fdd324
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105390"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/policies/featureRolloutPolicies/df85e4d9-e8c4-4033-a41c-73419a95c29c/appliesTo/2441b489-4f12-4882-b039-8f6006bd66da/$ref')
    .delete();

```