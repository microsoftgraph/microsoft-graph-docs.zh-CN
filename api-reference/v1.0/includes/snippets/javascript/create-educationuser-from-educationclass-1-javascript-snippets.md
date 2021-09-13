---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 12b49567c3abec6bbaea82b7c85f8b1174e829d3148752c598324df50b13b53f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277529"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationUser = {
  '@odata.id':'https://graph.microsoft.com/v1.0/education/users/13015'
};

await client.api('/education/classes/{class-id}/members/$ref')
    .post(educationUser);

```