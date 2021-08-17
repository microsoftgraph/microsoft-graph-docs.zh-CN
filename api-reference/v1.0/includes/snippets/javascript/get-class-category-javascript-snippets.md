---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f9e48219f9ad4ffa50c5b07b5e96222c04ffaf1aafa57680a6ce6298aae0cf8b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163858"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let educationCategory = await client.api('/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignmentCategories/96821157-5efb-4706-8ca2-a90b26c44852')
    .get();

```