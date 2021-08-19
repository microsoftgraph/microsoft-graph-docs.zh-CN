---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dbfbd79cee395d75288841f6c19800a1982d5321d76cadd91722a2a8adc34f10
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277648"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let contacts = await client.api('/me/contacts')
    .get();

```