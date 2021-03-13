---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ba347128e19f9f69b92854beb76d17bfc6f60b66
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50773821"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const sourceCollection = {
    displayName: 'Quarterly Financials search',
    contentQuery: 'subject:\'Quarterly Financials\'',
    'custodianSources@odata.bind': [
        'https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/custodians/2192ca408ea2410eba3bec8ae873be6b/userSources/46384443-4137-3032-3437-363939433735'
    ]
};

await client.api('/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/sourceCollections')
    .version('beta')
    .post(sourceCollection);

```