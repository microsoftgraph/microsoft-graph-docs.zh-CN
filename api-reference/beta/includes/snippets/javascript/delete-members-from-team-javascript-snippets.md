---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ba02590bcb5853cff9505d534eadf04c4c4a851caade17d88737b976cbce6afd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106598"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/teams/ee0f5ae2-8bc6-4ae5-8466-7daeebbfa062/members/ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=')
    .version('beta')
    .delete();

```