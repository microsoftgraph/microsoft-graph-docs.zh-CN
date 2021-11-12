---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9e5837a61358ec7f940b893f8344c4155fcd9284e2ffba28edfb34cc13367e19
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220220"
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
    .version('beta')
    .post(sectionGroup);

```