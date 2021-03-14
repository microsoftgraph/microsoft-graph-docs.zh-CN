---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 40e87e9cc16e1ae09b07a44e2f368956205926ba
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50793591"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let groupSetting = await client.api('/groupSettings/{id}')
    .get();

```