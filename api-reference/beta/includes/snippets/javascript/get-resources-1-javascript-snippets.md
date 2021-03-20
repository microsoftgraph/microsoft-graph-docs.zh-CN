---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8c459a60fcb415792b00b3c3fbec4f6788fc92a8
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50951788"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let resources = await client.api('/education/classes/11012/assignments/19002/resources')
    .version('beta')
    .get();

```