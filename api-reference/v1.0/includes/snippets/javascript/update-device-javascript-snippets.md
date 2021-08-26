---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 41352f9f050f2517c49642ffdcc7f43a2009bf735c92d400caee8ae7bd109a87
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278593"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const device = {
  accountEnabled: false
};

await client.api('/devices/{id}')
    .update(device);

```