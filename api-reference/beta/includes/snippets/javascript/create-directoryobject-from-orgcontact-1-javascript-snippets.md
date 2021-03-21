---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 861596bb8f2541b4c89a236a134ebd7b72f1879c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50957685"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
  directoryObject: {
  }
};

await client.api('/contacts/{id}/directReports')
    .version('beta')
    .post(directoryObject);

```