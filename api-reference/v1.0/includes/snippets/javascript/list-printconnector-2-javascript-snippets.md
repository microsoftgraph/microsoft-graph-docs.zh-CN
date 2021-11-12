---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a0a5bacf6b54526f759778a8bf268941b016363d62847493258a8e646c457587
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409686"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let connectors = await client.api('/print/printers/{printerId}/connectors')
    .get();

```