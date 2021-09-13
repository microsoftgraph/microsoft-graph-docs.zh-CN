---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 49d8c6bba4a40c1bdc9b0d8fae6490c3a639433a056b8d471b8cf223c361dff3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409322"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let place = await client.api('/places/3162F1E1-C4C0-604B-51D8-91DA78989EB1')
    .get();

```