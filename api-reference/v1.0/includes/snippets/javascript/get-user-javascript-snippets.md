---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 6238833d36eca4a43d20e03d0709699e3188a6eb
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36331219"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/me/user')
    .get();

```