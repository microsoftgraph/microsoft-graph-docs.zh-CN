---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d3d3f503a3bcd6f34a9ad5d08d343fc4f96b94205c41d92342228e594e8b8373
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56904303"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let onlineMeetings = await client.api('/communications/onlineMeetings/')
    .filter('VideoTeleconferenceId eq \'123456789\'')
    .get();

```