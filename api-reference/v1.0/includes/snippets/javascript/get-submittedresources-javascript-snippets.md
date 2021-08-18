---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 61097e7b20d29c05ae51ccc9b6e633d6f831def622e61d52ec080fca4f6b1367
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163856"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let submittedResources = await client.api('/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/ad8afb28-c138-4ad7-b7f5-a6986c2655a8/submissions/fbe51c90-78b7-418a-b5f3-871bf8d8d21e/submittedResources')
    .get();

```