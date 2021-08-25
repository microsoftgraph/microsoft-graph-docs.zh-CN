---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 39c542b39e4bdec631defc7bfc3148e77e3f9bf1
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2021
ms.locfileid: "58514491"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let directorySettingTemplate = await client.api('/directorySettingTemplates/08d542b9-071f-4e16-94b0-74abb372e3d9')
    .version('beta')
    .get();

```