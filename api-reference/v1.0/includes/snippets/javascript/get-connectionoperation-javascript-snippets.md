---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e8019880f3b4f878a846a739cc97a3f0593a0e3c3e44d5368817d8244b15878a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279188"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let connectionOperation = await client.api('/connections/contosohr/operations/3ed1595a-4bae-43c2-acda-ef973e581323')
    .get();

```