---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7ce8ac3d6416c1d50cc7e491d7f57c9c8142fc2e
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65315809"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let richLongRunningOperation = await client.api('/sites/root/operations/contentTypeCopy,0x010100298A15181454D84EBB62EDD7559FCBFE')
    .get();

```