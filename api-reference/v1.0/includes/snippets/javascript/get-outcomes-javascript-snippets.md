---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: de4174e47400ca748f2b3695542d2b1278cd216d
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52992615"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let outcomes = await client.api('/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/cf6005fc-9e13-44a2-a6ac-a53322006454/submissions/d1bee293-d8bb-48d4-af3e-c8cb0e3c7fe7/outcomes')
    .get();

```