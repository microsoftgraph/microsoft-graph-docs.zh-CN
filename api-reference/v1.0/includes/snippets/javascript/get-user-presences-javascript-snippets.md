---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6c9c799bcfc6723234a22b8c289eac3c73ae8cadad903163d7604d5c50fee83d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219316"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let presence = await client.api('/communications/presences/dc74d9bb-6afe-433d-8eaa-e39d80d3a647')
    .get();

```