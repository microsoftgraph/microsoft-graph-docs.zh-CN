---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8989181f0bd0baaafbab51d21deef833085b2f2807524c4a763199963d8c1eed
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903682"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const sectionGroup = {
  displayName: 'Section group name'
};

await client.api('/me/onenote/notebooks/{id}/sectionGroups')
    .version('beta')
    .post(sectionGroup);

```