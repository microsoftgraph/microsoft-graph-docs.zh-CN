---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 58a23f9b7ec11359d399a6d318eb6655ce7b1de9
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35856455"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/mailFolders/{id}/messages')
    .get();

```