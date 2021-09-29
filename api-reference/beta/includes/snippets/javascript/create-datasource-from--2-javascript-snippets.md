---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7fca19de4b63d69f41d5503ba6ab2fb746f3f933ee191444c426c3a3e34414cd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332514"
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