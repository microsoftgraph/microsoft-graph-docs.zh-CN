---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 00aee876d9078823a5c305856152d3aaf1b3c081
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/30/2019
ms.locfileid: "35932669"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/drive/items/{bundle-id}?expand=children')
    .version('beta')
    .get();

```