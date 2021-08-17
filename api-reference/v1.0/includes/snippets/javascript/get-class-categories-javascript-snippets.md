---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2a8c9133f457d7c1f7098382298e28a390f99ff9e1c820a9c7723d6096f1039a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333794"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let assignmentCategories = await client.api('/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignmentCategories')
    .get();

```