---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2ebe7543a319eb7d44523360b4211b27e4e5aae10f82be65be599548f88b6f76
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332963"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/print/taskDefinitions/{printTaskDefinitionId}')
    .delete();

```