---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c6a69097c40d8db23d889beacc31c16dd384257d
ms.sourcegitcommit: 1585d55d3e7030b5fd1f7cfd5de8f9fb8202cd56
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/09/2019
ms.locfileid: "37428852"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const copyNotebookModel = {webUrl:"webUrl value"};

let res = await client.api('/me/onenote/notebooks/GetNotebookFromWebUrl')
    .post(copyNotebookModel);

```