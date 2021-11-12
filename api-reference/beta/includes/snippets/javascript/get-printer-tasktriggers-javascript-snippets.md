---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 71075289552531bd571d3a33fcb2d30f370ecf098c4201ce04bf3f240b717870
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163104"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let taskTriggers = await client.api('/print/printers/{id}/taskTriggers')
    .version('beta')
    .get();

```