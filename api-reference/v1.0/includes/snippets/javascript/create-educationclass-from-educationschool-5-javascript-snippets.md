---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c63b2f427cf8e8c2211e553fcc6bf992c72a5d92e7184f01168171607414691e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329092"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationClass = {
 '@odata.id':'https://graph.microsoft.com/v1.0/education/classes/11006'
};

await client.api('/education/schools/{school-id}/classes/$ref')
    .post(educationClass);

```