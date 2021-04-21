---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3859e2648aefcd54cf5400b8f2869ee0e302805f
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51920142"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let b2xUserFlows = await client.api('/identity/b2xUserFlows')
    .get();

```