---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dab65c7a9478aa5ba171a0841f69f5a4c531645b
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/10/2021
ms.locfileid: "50179526"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/schools/10002/classes')
    .version('beta')
    .get();

```