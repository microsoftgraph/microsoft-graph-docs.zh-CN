---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dc26b12d8ba14fe7c42af0029f9abb276369ed78
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52990769"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
    '@odata.id': 'https://graph.microsoft.com/beta/directoryObjects/bb165b45-151c-4cf6-9911-cd7188912848'
};

await client.api('/directoryRoles/roleTemplateId=88d8e3e3-8f55-4a1e-953a-9b9898b8876b/members/$ref')
    .version('beta')
    .post(directoryObject);

```