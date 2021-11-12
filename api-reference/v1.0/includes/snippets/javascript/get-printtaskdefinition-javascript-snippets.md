---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b4eaf18afba3a7da23a76372c44e71111d5de19eee04bbeb23ad5a33da6fbc62
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219307"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let printTaskDefinition = await client.api('/print/taskDefinitions/{printTaskDefinitionId}')
    .get();

```