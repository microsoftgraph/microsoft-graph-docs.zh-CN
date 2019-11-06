---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 093f3eccc14ea7f6a9d2d33b9efc0ef0d2d594d8
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37997211"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const personName = {
  displayName: "displayName-value",
  first: "first-value",
  initials: "initials-value",
  last: "last-value",
  languageTag: "languageTag-value",
  maiden: "maiden-value"
};

let res = await client.api('/me/profile/names/{id}')
    .version('beta')
    .update(personName);

```