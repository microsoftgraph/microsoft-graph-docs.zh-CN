---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7d63bb0ab0772c2af169059dfcbe4b09c1c62b90
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50805971"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let groupSettingTemplates = await client.api('/groupSettingTemplates')
    .get();

```