---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b4f8dcace3bb1d1c4633703a7412839aec1164bb
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50946320"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let custodian = await client.api('/compliance/ediscovery/cases/2192ca408ea2410eba3bec8ae873be6b/custodians/45454331323337443946343043464239')
    .version('beta')
    .get();

```