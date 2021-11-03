---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 80a9920a72aa421f7bff2e7deded26746d5a496c8b3380b67abf1839da3e240c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104157"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let accessReviews = await client.api('/accessReviews')
    .version('beta')
    .filter('businessFlowTemplateId eq \'6e4f3d20-c5c3-407f-9695-8460952bcc68\'')
    .skip(0)
    .top(100)
    .get();

```