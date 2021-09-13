---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 39562e02da948faff8804663899df251ca23b688723b45dfc421bf8f94731fe9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902212"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let team = await client.api('/teams/893075dd-2487-4122-925f-022c42e20265')
    .get();

```