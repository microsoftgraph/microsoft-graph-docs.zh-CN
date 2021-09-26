---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8193c945875649a06fc4c9b12b1eb033236f481e44a75db8fc6abd7e2d875702
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279017"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let onPremisesConnections = await client.api('/deviceManagement/virtualEndpoint/onPremisesConnections')
    .version('beta')
    .get();

```