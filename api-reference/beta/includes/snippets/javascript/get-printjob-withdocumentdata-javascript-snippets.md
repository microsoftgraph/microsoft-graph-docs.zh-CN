---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4761a250a863dda67b50237370c375016f99134e
ms.sourcegitcommit: 2050639c9e9a6b2dab9ce53d6a9fc87e98789b50
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/08/2020
ms.locfileid: "45080607"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/print/printers/86b6d420-7e6b-4797-a05c-af4e56cd81bd/jobs/31216')
    .version('beta')
    .expand('documents')
    .get();

```