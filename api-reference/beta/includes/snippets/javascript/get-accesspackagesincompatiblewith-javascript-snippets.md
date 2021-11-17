---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9957db86209e0dbeb9b6eb8c3dc1a15793a8091e35990cdc35519b82acf182d7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902833"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let accessPackagesIncompatibleWith = await client.api('/identityGovernance/entitlementManagement/accessPackages/{id}/accessPackagesIncompatibleWith')
    .version('beta')
    .get();

```