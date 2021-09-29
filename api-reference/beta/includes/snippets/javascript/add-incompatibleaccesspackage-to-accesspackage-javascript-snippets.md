---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8b1ce80cdf088f68e334e1eda99d8e5a49d780267ad47a947e69adc2a6682813
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104210"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const accessPackage = {
    '@odata.id': 'https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/c0a74b4d-2694-4d5d-a964-1bee4ff0aaf2'
};

await client.api('/identityGovernance/entitlementManagement/accessPackages/{id}/incompatibleAccessPackages/$ref')
    .version('beta')
    .post(accessPackage);

```