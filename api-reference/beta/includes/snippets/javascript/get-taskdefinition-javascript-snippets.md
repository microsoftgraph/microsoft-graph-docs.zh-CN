---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 39ae47598cc57829789a4831e249300f6863c6de677ec64d9a74ea398013bb7d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105537"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let printTaskDefinition = await client.api('/print/taskDefinitions/fab143fd-ee61-4358-8558-2c7dee953982')
    .version('beta')
    .get();

```