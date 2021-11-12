---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: abe185376981e6a55c15e026a42dd1cf3c933434c50a97fc4d937b8dc6903185
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902491"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let connectors = await client.api('/print/printers/{id}/connectors')
    .version('beta')
    .get();

```