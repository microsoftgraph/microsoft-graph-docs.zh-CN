---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 89342c4366327a747906dc09d0e9a5c86da4e360
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40871113"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/communications/calls/7531d31f-d10d-44de-802f-c569dbca451c/participants')
    .get();

```