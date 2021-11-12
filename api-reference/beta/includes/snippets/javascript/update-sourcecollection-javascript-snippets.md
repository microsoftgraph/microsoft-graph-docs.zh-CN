---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a855fc1de43f951b1bd81a6c1aa1d50f0d320897bfa6cd0f8f8f2412a93e03b1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106165"
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