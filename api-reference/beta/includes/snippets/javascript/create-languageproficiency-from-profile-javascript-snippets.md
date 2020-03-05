---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2e4ba9af62e42dfd254f8503a9ab9324041be8bd
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "37996553"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const languageProficiency = {
  displayName: "displayName-value",
  tag: "tag-value",
  proficiency: "proficiency-value"
};

let res = await client.api('/me/profile/languages')
    .version('beta')
    .post(languageProficiency);

```