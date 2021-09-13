---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bbdad68090d029cfeb859d43c7aaa958a955380056044b2811855953ce23c432
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332646"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/contacts/{id}')
    .delete();

```