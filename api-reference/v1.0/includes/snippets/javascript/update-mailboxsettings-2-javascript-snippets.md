---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b667768e806b69cee7b094eaa36b7a952e7a78ac
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50475504"
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