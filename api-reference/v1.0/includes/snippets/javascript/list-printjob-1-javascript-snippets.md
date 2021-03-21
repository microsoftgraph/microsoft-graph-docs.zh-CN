---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e1dfd594a8db6d09b0dee8d70c737711c7f44cb7
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50956282"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let jobs = await client.api('/print/printers/{printerId}/jobs')
    .get();

```