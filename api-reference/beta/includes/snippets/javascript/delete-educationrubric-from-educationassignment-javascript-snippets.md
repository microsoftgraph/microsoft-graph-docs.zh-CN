---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 12500d1c75ac3cba9a21ac8cbedc52e957d64d0dd5d924e9f7f53892d19a06fb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332506"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/education/classes/{id}/assignments/{id}/rubric/$ref')
    .version('beta')
    .delete();

```