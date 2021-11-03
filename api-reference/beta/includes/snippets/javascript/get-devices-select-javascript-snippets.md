---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d81ff043a02b7c826c469904295a648020409c5a
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60694555"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let devices = await client.api('/devices')
    .version('beta')
    .select('id,extensionAttributes')
    .get();

```