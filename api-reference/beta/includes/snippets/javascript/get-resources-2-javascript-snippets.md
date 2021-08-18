---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f93b9f52413e253e7f7c01fafce080cb88d697d24ccb4aa9f10dc57ec4b623ff
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163993"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let resources = await client.api('/education/classes/{id}/assignments/{id}/submissions/{id}/resources')
    .version('beta')
    .get();

```