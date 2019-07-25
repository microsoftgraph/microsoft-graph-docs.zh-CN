---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 2bd79a292c0b0435678673b32bd6a2881da4e1dd
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35706340"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/directorySettingTemplates')
    .version('beta')
    .get();

```