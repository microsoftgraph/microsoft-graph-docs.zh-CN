---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0ed8b30b7209a4de08bfb7087c26e13a40340924
ms.sourcegitcommit: fa08172601324fc01b090f8135fba4600bd1a9f8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/13/2019
ms.locfileid: "38302676"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const subscribeToToneOperation = {
  clientContext: "fd1c7836-4d84-4e24-b6aa-23188688cc54"
};

let res = await client.api('/communications/calls/{id}/subscribeToTone')
    .version('beta')
    .post(subscribeToToneOperation);

```