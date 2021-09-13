---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b01caad2f2260a1557f3bcadb9b339ca4962f3b593838773ce84998fe364c656
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57107106"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const cancelMediaProcessingOperation = {
  clientContext: 'clientContext-value'
};

await client.api('/communications/calls/{id}/cancelMediaProcessing')
    .post(cancelMediaProcessingOperation);

```