---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 92ffa9e892127c36dd9ab18cde89cddb64302d8a1e1c5f8d4b2ed728f0c7c882
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279270"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let attachments = await client.api('/groups/1848753d-185d-4c08-a4e4-6ee40521d115/threads/AAQkADJfolA==/posts/AAMkADJ-aHAAA=/attachments')
    .version('beta')
    .get();

```