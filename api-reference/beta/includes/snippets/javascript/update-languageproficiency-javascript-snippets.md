---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 502b1a55bc4dbe045b6a4c84bab19517ca32bd13
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37998240"
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

let res = await client.api('/me/profile/languages/{id}')
    .version('beta')
    .update(languageProficiency);

```