---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f62fbbc1e5676dcb78b643fc9d429d9eab76ec4818c335bc695cc0e89f25fef4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163082"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const publishedResource = {
    displayName: 'New provisioning',
    resourceName: 'domain1.contoso.com'
};

await client.api('/onPremisesPublishingProfiles/provisioning/publishedResources')
    .version('beta')
    .post(publishedResource);

```