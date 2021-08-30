---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7c9353ae842155a05a37297485fda305c9733fd9294cb1e50a4c4205f1b2b72e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221121"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/external/connections/contosohr/groups/31bea3d537902000')
    .version('beta')
    .delete();

```