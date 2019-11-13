---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 13255402109cee7203873d8027fdec2dcaa94bf8
ms.sourcegitcommit: fa08172601324fc01b090f8135fba4600bd1a9f8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/13/2019
ms.locfileid: "38302539"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896')
    .version('beta')
    .delete();

```