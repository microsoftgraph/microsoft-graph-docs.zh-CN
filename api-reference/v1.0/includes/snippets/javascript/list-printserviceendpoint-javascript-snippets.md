---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f9f532d0b3b098b27f2ff4cc86a0a30fbdde10dd0278da47c54cd79639785a03
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220394"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let endpoints = await client.api('/print/services/{printServiceId}/endpoints')
    .get();

```