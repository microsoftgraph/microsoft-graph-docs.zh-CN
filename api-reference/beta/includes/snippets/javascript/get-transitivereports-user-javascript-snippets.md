---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dc74fa5c39aa765cf92d10f9442e6cbafa79f1367b05a96d698f9feacb3b370f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332350"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let int32 = await client.api('/users/45b7d2e7-b882-4a80-ba97-10b7a63b8fa4/transitiveReports/$count')
    .version('beta')
    .get();

```