---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 231f518a781a8488b63bc2aa15deaed59ee39f92d5d8434589b50c1f64e4ac8c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378283"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/education/synchronizationProfiles/{id}/start')
    .version('beta')
    .post();

```