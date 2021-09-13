---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8d6c252bbd49f31ad48c82d761a5b8d8fbffc456ebd189b3a6c957254e1504a6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219332"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let sectionGroups = await client.api('/me/onenote/sectionGroups')
    .get();

```