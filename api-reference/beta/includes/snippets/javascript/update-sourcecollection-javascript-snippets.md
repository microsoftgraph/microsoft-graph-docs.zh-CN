---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d6ee4d9df5a618924b959cd93348e179558debfb
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50776527"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const sourceCollection = {
    displayName: 'Quarterly Financials search',
};

await client.api('/compliance/ediscovery/cases/{caseId}/sourceCollections/1a9b4145d8f84e39bc45a7f68c5c5119')
    .version('beta')
    .update(sourceCollection);

```