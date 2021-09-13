---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 85f96b9f1910200934f74d7f1da709ef98616c2ad1df3cb62dfe7263f9196544
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333827"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/education/schools/{school-id}/classes/{class-id}')
    .delete();

```