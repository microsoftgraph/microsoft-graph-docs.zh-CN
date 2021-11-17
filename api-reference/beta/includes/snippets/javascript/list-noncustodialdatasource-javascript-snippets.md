---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4f731ccd4f38fa0aa2efb934893eb993bea95d84c8022f202363b1dce68d7562
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57103880"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let noncustodialDataSources = await client.api('/compliance/ediscovery/cases/5b840b94-f821-4c4a-8cad-3a90062bf51a/noncustodialDataSources')
    .version('beta')
    .get();

```