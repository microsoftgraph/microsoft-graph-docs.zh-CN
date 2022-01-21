---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bca3b9ab8165163af56c4c64d73315e9f541c904
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62094536"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const bookingCustomQuestion = {
  '@odata.type': '#microsoft.graph.bookingCustomQuestion',
  displayName: 'What is your age?',
  answerInputType: 'text',
  answerOptions: []
};

await client.api('/bookingBusinesses/Contosolunchdelivery@contoso.onmicrosoft.com/customQuestions/3bc6fde0-4ad3-445d-ab17-0fc15dba0774')
    .version('beta')
    .update(bookingCustomQuestion);

```