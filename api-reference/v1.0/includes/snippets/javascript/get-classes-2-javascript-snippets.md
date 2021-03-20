---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8aae7b3678e64b45cf2033ef8b2331aed3397109
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50945386"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let classes = await client.api('/education/schools/{school-id}/classes')
    .get();

```