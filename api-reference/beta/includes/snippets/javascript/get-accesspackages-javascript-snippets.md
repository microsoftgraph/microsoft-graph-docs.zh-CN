---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cd3ecddeb2599fb9432794019966b0b713a028ad5297531e438984242c05939d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104220"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let accessPackages = await client.api('/identityGovernance/entitlementManagement/accessPackages')
    .version('beta')
    .get();

```