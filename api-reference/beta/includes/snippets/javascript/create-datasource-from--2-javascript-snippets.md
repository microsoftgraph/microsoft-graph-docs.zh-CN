---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9a8d8220c5badf8f3f7c4596d5b9bf238326f9ba
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50952038"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const dataSource = {
  '@odata.id':'https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/custodians/ab3a628a383045eba344b3caecba3104/userSources/31423539-3846-4333-4136-353644383531'
};

await client.api('/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/sourceCollections/1a9b4145d8f84e39bc45a7f68c5c5119/custodianSources/$ref')
    .version('beta')
    .post(dataSource);

```