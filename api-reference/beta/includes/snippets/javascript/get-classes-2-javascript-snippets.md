---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aae1e0146c86cf965310672af06f8d867c7b882bcb03a2f5464aeaebc8d6cfc4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220105"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let classes = await client.api('/education/schools/10002/classes')
    .version('beta')
    .get();

```