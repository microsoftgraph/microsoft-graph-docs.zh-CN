---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a50ae90355d222dbb398974eb538f5ef794f844b
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865840"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const reject = {
  reason: "none"
};

let res = await client.api('/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/reject')
    .post(reject);

```