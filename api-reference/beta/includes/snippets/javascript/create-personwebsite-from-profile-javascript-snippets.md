---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8cd12fb4f48e9f7771db5a965cc8a01cb342d6ef
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/20/2020
ms.locfileid: "46821404"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const personWebsite = {
  categories: [
    "football"
  ],
  displayName: "Lyn Damer",
  webUrl: "www.lyndamer.no"
};

let res = await client.api('/me/profile/websites')
    .version('beta')
    .post(personWebsite);

```