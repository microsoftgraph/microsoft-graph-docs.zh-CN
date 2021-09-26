---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d0aa47cab8d51e96240c7fe0d5100fd1be816675
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59763899"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const externalDomainName = {
    '@odata.type': 'microsoft.graph.externalDomainName',
    id: 'contososuites.com'
};

await client.api('/directory/federationConfigurations/d5a56845-6845-d5a5-4568-a5d54568a5d5/microsoft.graph.samlOrWsFedExternalDomainFederation/domains')
    .version('beta')
    .post(externalDomainName);

```