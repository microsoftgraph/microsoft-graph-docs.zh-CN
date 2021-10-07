---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ad19fb559bae09b4a7a355ca0e3e409d18c2b0e53bc11db5e599ebc2a9bef989
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332403"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/education/classes/11021/assignments/19002/submissions/850f51b7/resources/f2387c3b-ec39-4bf2-a399-d7242677f024')
    .version('beta')
    .delete();

```