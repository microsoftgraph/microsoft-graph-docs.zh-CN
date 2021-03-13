---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4b98b8931a47bb3bcb2b8821917d109c576a0e5e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50772112"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let printConnector = await client.api('/print/connectors/{printConnectorId}')
    .get();

```