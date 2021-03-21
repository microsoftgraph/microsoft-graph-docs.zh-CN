---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5612f7bfa53ef6c76a89023efde9b56b89e6e17b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962287"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let services = await client.api('/print/services')
    .version('beta')
    .get();

```