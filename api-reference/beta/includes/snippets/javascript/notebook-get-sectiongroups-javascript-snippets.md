---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d1f8e6b19fb88ca4e023144762795d9301b6b8746d33c6fef2a75c8548337740
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332888"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let sectionGroups = await client.api('/me/onenote/notebooks/{id}/sectionGroups')
    .version('beta')
    .get();

```