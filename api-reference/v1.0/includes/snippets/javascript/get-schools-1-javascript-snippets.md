---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d217ac96a392d895e40c16f2b3b5017400d496f1
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50963793"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let schools = await client.api('/education/classes/{class-id}/schools')
    .get();

```