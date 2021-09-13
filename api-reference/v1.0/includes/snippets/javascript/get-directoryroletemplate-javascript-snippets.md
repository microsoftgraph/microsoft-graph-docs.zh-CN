---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8fae66a85001d21a72b8d22f76d1eea623bb1f6a80bd43cf2c1469309cca885b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277544"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let directoryRoleTemplate = await client.api('/directoryRoleTemplates/{id}')
    .get();

```