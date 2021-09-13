---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5c84aaaaae453343eb9a1fd70820653e127c6de722f39e8eec081bee34be4255
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162557"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let attachments = await client.api('/groups/1848753d-185d-4c08-a4e4-6ee40521d115/threads/AAQkADJfolA==/posts/AAMkADJ-aHAAA=/attachments')
    .get();

```