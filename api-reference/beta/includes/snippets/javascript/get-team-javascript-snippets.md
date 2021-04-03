---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6b16cd9490738328b6486e73385f06d5385f3abf
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51507413"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let team = await client.api('/teams/893075dd-2487-4122-925f-022c42e20265')
    .version('beta')
    .get();

```