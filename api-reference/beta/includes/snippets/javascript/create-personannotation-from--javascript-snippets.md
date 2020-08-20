---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 87c79ccffe39184fd56f592606dff9da0fef0462
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/20/2020
ms.locfileid: "46820198"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const personAnnotation = {
  detail: {
    contentType: "text",
    content: "I am originally from Australia, but grew up in Moscow, Russia."
  },
  displayName: "About Me"
};

let res = await client.api('/me/profile/notes')
    .version('beta')
    .post(personAnnotation);

```