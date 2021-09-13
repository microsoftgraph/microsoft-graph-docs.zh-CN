---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 65d432b0d3bce7a597013690b31adb5cb51aae95d4a7199148e3eda1be4fad80
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220261"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const personAnnotation = {
  allowedAudiences: 'organization'
};

await client.api('/users/{userId}/profile/notes/{id}')
    .version('beta')
    .update(personAnnotation);

```