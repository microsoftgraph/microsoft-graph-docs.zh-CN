---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bd26efaea565f9237863952cd09765dea44e1cb0
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50788821"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let acceptedSenders = await client.api('/groups/{id}/acceptedSenders')
    .get();

```