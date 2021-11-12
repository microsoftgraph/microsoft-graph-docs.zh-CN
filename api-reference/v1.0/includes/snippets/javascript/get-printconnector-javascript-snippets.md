---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c00b4ca8cc84e0d45c657b0de0f3915d6355fdc09e3f10907bfbd8b5598c7ac7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409331"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let printConnector = await client.api('/print/connectors/{printConnectorId}')
    .get();

```