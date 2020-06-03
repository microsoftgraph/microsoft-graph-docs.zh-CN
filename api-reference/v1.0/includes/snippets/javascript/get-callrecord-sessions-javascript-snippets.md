---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7929cb7ed45e945f647dbb49ff17fc86a7ba1b90
ms.sourcegitcommit: 43f7800894857a29f02fffaf4a50ad6386b5bf59
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/03/2020
ms.locfileid: "44524552"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/communications/callRecords/{id}/sessions')
    .get();

```