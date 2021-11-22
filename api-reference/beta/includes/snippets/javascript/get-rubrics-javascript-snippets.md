---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 864cffd8742fda4b892b982977d102ccc048554a69128f722d59745ffabc879b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163696"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let rubrics = await client.api('/education/me/rubrics')
    .version('beta')
    .get();

```