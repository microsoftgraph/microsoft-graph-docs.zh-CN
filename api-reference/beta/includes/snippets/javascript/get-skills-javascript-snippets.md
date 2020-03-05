---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6e5a60ffd2e5e9d4c4c76822a6aae2d6b01e4698
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "37997898"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/profile/skills')
    .version('beta')
    .get();

```