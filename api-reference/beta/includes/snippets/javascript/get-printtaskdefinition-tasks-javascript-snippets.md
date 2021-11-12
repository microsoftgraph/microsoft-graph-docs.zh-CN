---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 90b012f52b11652bf8e23e8ee16b7d68e9b7dce31cb82e91402bc19b3f890a10
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158494"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let tasks = await client.api('/print/taskDefinitions/92d72a3d-cad7-4809-8924-43833282b079/tasks')
    .version('beta')
    .get();

```