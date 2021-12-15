---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d28e609993eee32f18e9e79e8afc4bb5e0532cd7
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/15/2021
ms.locfileid: "61525846"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let submissions = await client.api('/education/classes/59069eb2-2a09-4d90-bb19-2089cc69d613/assignments/80da1069-a635-4913-813f-d775a5470a8f/submissions')
    .version('beta')
    .header('Prefer','include-unknown-enum-members')
    .get();

```