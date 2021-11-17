---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fb71e6173660b95d353698b95bee01286bf8ce95f45d32323bda67b69ec63d83
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162458"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const program = {
    displayName: 'testprogram3',
    description: 'test description'
};

await client.api('/programs')
    .version('beta')
    .post(program);

```