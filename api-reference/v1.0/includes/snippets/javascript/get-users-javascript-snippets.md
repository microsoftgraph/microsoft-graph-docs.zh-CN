---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d203eb57d70a48d391d7ae884084071a5e786530
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "35730258"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users')
    .get();

```