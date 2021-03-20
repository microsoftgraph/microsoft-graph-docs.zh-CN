---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aa1633b2c2a8539e644f19a90202539574579512
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50949616"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let organization = await client.api('/organization')
    .get();

```