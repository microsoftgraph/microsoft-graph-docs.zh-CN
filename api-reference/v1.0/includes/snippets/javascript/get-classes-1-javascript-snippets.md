---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 815ef94c9c09f71e2bb35dff9eedd2a0f589437f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50956659"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let classes = await client.api('/education/classes')
    .get();

```