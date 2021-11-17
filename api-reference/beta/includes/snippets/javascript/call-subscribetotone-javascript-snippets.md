---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e0d07c0f282534f7ecd3b8d8ce73a6ecd68da3b75247e010fc9c160849570610
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105253"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const subscribeToToneOperation = {
  clientContext: 'fd1c7836-4d84-4e24-b6aa-23188688cc54'
};

await client.api('/communications/calls/{id}/subscribeToTone')
    .version('beta')
    .post(subscribeToToneOperation);

```