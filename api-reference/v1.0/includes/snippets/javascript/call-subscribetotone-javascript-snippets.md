---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c1f892752ed13e771f1cb0bd7db87da827d1c9270f840218cf488d89b37a1cb9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378802"
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
    .post(subscribeToToneOperation);

```