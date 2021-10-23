---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3f2c415abc14727a879e1be3a3f96ea94a501532ad2b8e1eeef88a9ee367ca04
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215861"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/compliance/ediscovery/cases/{caseId}/settings/resetToDefault')
    .version('beta')
    .post();

```