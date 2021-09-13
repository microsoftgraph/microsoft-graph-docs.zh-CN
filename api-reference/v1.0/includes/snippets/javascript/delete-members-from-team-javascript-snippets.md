---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2300ef189f9078554c4913f486bc08062dccb355a187c30618d696847ed4af3e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277845"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/teams/ee0f5ae2-8bc6-4ae5-8466-7daeebbfa062/members/ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=')
    .delete();

```