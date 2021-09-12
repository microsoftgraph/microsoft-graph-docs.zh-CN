---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4624943fd3dc6c0749438ed187d9f3c08d3e3189750ddb2930d265ba47f7588b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105294"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let calendars = await client.api('/me/calendars')
    .get();

```