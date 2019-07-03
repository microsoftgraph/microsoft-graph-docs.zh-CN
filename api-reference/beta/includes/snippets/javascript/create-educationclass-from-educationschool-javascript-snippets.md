---
description: 自动生成的文件。 不修改
ms.openlocfilehash: cef07a40c27b4fd3ccccd16fe1daffc1fe9dfe5e
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35520141"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationClass = {
 @odata.id:"https://graph.microsoft.com/beta/education/classes/11006"
};

let res = await client.api('/education/schools/10002/classes/$ref')
    .version('beta')
    .post({educationClass : educationClass});

```