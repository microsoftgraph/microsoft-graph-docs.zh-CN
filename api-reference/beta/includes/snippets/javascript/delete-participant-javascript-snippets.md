---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 67036ac8842fbfa01a72781965296ae181be1aadb70b3ba575e513dd05778542
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278163"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/communications/calls/{id}/participants/{id}')
    .version('beta')
    .delete();

```