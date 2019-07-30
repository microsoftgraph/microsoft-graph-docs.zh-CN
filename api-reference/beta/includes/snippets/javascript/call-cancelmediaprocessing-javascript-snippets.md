---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 62ba0d30ac12d06d585324c732f9bd0c29ce89a0
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/30/2019
ms.locfileid: "35933803"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const cancelMediaProcessingOperation = {
  all: true,
  clientContext: "clientContext-value"
};

let res = await client.api('/app/calls/{id}/cancelMediaProcessing')
    .version('beta')
    .post(cancelMediaProcessingOperation);

```