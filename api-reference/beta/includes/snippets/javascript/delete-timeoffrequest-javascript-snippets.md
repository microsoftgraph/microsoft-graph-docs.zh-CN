---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0426e8eb7d559ff0779454ca73b3b37c8a0e5b88
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40863590"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teams/{id}/schedule/timeOffRequests')
    .version('beta')
    .delete();

```