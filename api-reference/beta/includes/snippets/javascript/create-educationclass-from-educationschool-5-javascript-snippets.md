---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6cc340a099a1801835bba42af3b326b96d6fde7f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50951295"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationClass = {
 '@odata.id':'https://graph.microsoft.com/beta/education/classes/11006'
};

await client.api('/education/schools/10002/classes/$ref')
    .version('beta')
    .post(educationClass);

```