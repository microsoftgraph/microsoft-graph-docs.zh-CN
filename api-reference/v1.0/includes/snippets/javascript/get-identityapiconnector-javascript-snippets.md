---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fc201d054d7de746f7d84dafd344742849a2aa9b95226dc678a6b43f5d2f38b0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56904314"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let identityApiConnector = await client.api('/identity/apiConnectors/370eeb68-dfd3-4a47-8160-8824c2358321')
    .get();

```