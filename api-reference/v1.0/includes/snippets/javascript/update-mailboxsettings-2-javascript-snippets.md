---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a54d1387bd25fb7788886e0e396a1616a875a7c90608b91d490d8b92ace3e9b3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218374"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const mailboxSettings = {
  workingHours: {
      endTime: '18:30:00.0000000', 
      daysOfWeek: [ 
          'Monday', 
          'Tuesday', 
          'Wednesday', 
          'Thursday', 
          'Friday', 
          'Saturday' 
      ], 
      timeZone: { 
         '@odata.type': '#microsoft.graph.customTimeZone', 
         bias: -300, 
         name: 'Customized Time Zone',
         standardOffset: {   
           time: '02:00:00.0000000', 
           dayOccurrence: 2, 
           dayOfWeek: 'Sunday', 
           month: 10, 
           year: 0 
         }, 
         daylightOffset: {   
           daylightBias: 100, 
           time: '02:00:00.0000000', 
           dayOccurrence: 4, 
           dayOfWeek: 'Sunday', 
           month: 5, 
           year: 0 
         } 
      } 
  }
};

await client.api('/me/mailboxSettings')
    .update(mailboxSettings);

```