---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fb838f8c199fcb0dfc39f8b353ee8c6a9822e9ae4debeae638c5766f879d1630
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219227"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let educationRubric = await client.api('/education/me/rubrics/{id}')
    .version('beta')
    .get();

```