---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e60fc327c077c0ed40c4109f813e136499d1bff5
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50953815"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let lists = await client.api('/me/todo/lists')
    .version('beta')
    .get();

```