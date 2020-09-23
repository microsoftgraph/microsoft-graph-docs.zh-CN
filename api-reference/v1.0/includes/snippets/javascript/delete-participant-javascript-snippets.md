---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 62699c3f01f375926f7b1d661ffb704991a0a810
ms.sourcegitcommit: a3fc420a5639c0f4e89af2b602db17392e176802
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/23/2020
ms.locfileid: "48222841"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/communications/calls/{id}/participants/{id}')
    .delete();

```