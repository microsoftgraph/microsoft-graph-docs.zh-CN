---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8239be705c39bac5b9687e78c33222aff63bfc60
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40869357"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teams/{id}/schedule/openShifts')
    .version('beta')
    .delete();

```