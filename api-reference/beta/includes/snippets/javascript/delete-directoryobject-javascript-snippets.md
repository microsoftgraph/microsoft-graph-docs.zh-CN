---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4d44d49f5a6f9bc2fc0aa3e00227b55d25b6af6c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50769974"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/directoryObjects/ffab4dce-9b82-49a6-b7c7-1a143106598c')
    .version('beta')
    .delete();

```