---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 14a822c9073117e8612ba7824f7e8cb9527011254daf9cab1872ddbf371d83e4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163072"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let riskDetections = await client.api('/riskDetections')
    .version('beta')
    .get();

```