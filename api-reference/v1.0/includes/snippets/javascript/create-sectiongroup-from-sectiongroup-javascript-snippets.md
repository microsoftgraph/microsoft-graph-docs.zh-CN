---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fffc4c881ec6ad5a08cc05880cc2ad45e4de8706e6008093a7034cf9ab603454
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220384"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const sectionGroup = {
  displayName: 'Section group name'
};

await client.api('/me/onenote/sectionGroups/{id}/sectionGroups')
    .post(sectionGroup);

```