---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0172825a288152182ab19e5defe5b897d38681653d6c12aff3a302f1ea988c71
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215995"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let sections = await client.api('/me/onenote/notebooks/{id}/sections')
    .get();

```