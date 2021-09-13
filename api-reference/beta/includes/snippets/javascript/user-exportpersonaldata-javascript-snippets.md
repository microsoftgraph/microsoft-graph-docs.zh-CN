---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 44b632de1df581da3a7d843ae879f04e80883ce114f1d16a1c3547876c079cc9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215767"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const exportPersonalData = {
  storageLocation: 'storageLocation-value'
};

await client.api('/users/{id}/exportPersonalData')
    .version('beta')
    .post(exportPersonalData);

```