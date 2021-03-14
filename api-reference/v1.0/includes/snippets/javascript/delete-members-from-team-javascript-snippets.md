---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ce6648e4b6c928f7302201d1d5c07ee53d9e892e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50803562"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/teams/ee0f5ae2-8bc6-4ae5-8466-7daeebbfa062/members/ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=')
    .delete();

```