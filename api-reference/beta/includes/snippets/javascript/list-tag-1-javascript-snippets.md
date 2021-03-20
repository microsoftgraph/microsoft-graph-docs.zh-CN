---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cbc14ed16c190ad0f14c614e8832479b1e9171c3
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50946368"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let tags = await client.api('/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/tags')
    .version('beta')
    .get();

```