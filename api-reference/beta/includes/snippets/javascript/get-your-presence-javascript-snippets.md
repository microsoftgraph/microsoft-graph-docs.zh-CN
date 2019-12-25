---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 79468960532ebfffa22cad61af281230527e6a00
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40867684"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/presence')
    .version('beta')
    .get();

```