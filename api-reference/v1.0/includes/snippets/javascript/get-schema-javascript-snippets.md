---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 03a0f82ccdef9816b8ebf0337b30c2a417eefbee
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60694374"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let schema = await client.api('/external/connections/contosohr/schema')
    .get();

```