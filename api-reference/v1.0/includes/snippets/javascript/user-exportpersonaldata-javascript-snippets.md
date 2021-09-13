---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2d309e94df66f6b863201c69592770adc55cc806e85ce08b02a28d6f130d4adc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104267"
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
    .post(exportPersonalData);

```