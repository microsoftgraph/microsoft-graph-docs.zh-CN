---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cf6a04241e2c21d66b9bd203efe1b2345275e30f38d28a34320aec55144a9b5a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57164294"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let educationAssignmentResource = await client.api('/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/cf6005fc-9e13-44a2-a6ac-a53322006454/resources/8b01c1d0-aafc-4f8c-bd73-89faa3df1c1c')
    .get();

```