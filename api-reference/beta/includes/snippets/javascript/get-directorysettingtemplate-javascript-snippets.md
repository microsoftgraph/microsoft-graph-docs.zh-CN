---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e9aca11225022e41f7a26803b263796583eff6db
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48606721"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/directorySettingTemplates/{id}')
    .version('beta')
    .get();

```