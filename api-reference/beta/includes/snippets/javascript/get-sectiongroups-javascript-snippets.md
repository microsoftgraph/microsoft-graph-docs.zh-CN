---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1e3aa5d16585fc00be717edc60c418da73ed6632e999d53017f190216cc3ea0c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378637"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let sectionGroups = await client.api('/me/onenote/sectionGroups/{id}/sectionGroups')
    .version('beta')
    .get();

```