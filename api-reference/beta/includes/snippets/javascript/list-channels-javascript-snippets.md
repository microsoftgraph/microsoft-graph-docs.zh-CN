---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 18ad0d7a597a4ddfe6f61ba9ae232fd9a72541ae8a4bf6f11a123caa0acfacf0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163832"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let channels = await client.api('/teams/893075dd-2487-4122-925f-022c42e20265/channels')
    .version('beta')
    .get();

```