---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e14eb8137d0712d47da05eba8f6717ced6cede40
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50942322"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let printConnector = await client.api('/print/connectors/{id}')
    .version('beta')
    .get();

```