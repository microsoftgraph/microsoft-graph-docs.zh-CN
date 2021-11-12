---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8ac63821492f4b8fe945b8f5a5c06523c641e774432d0936ecd339e9acbe62e8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903515"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let taskDefinitions = await client.api('/print/taskDefinitions')
    .get();

```