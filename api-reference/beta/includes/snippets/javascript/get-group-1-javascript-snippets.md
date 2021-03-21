---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b0c7c2f003fd278b5a38b3644193eb4cb7244ddf
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50961800"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let group = await client.api('/groups/45b7d2e7-b882-4a80-ba97-10b7a63b8fa4')
    .version('beta')
    .get();

```