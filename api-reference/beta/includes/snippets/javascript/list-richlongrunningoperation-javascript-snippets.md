---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b73b8b30699c1d5cda0539e58fee9085ffe962ab
ms.sourcegitcommit: 871db8b3f68489d24e2aeafe694725579ee44c47
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2022
ms.locfileid: "62225906"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let operations = await client.api('/sites/{site-ID}/operations')
    .version('beta')
    .get();

```