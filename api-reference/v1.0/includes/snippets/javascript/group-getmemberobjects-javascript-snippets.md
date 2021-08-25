---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 001f05ea0706f4d634777a3720fa2cadb095a597
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2021
ms.locfileid: "58513319"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const string = {
  securityEnabledOnly: false
};

await client.api('/groups/1132b215-826f-42a9-8cfe-1643d19d17fd/getMemberObjects')
    .post(string);

```