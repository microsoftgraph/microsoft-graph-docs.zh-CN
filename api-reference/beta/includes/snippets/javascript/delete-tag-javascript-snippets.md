---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9dec97f69670371770268883bde2843696c6204190b1a2a6736ece5e98075153
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332512"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/tags/9985bd266f2f459cbebc81522734b452?forcedelete=true')
    .version('beta')
    .delete();

```