---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d6a475b103a8f020525b3362e5d0be2d44435a14a1ec3f77fd553602d47f639d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219128"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/policies/permissionGrantPolicies/my-custom-consent-policy')
    .version('beta')
    .delete();

```