---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b66c1742ab28ba3608cf5f8cd1ae2156def59831
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865794"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/communications/onlineMeetings/')
    .filter('VideoTeleconferenceId eq '123456789'')
    .get();

```