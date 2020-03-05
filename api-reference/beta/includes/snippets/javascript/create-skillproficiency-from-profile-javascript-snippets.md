---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a281c92d0985562235d8e65a08e2112f2cdf1579
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "37997758"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const skillProficiency = {
  categories: [
    "categories-value"
  ],
  displayName: "displayName-value",
  proficiency: "proficiency-value",
  webUrl: "webUrl-value"
};

let res = await client.api('/me/profile/skills')
    .version('beta')
    .post(skillProficiency);

```