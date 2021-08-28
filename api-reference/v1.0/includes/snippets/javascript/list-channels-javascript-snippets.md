---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9ae4fe109977acc9ef7f17a6c2c33441fa3847453a7bbde1bd00806fc9e3715d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163017"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let channels = await client.api('/teams/893075dd-2487-4122-925f-022c42e20265/channels')
    .get();

```