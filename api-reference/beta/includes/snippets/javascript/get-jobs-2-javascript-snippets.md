---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bd1186d73def470631e96e8012f4c4e144e8f1e86143781161633210343b53c1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161667"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let jobs = await client.api('/print/shares/{id}/jobs')
    .version('beta')
    .get();

```