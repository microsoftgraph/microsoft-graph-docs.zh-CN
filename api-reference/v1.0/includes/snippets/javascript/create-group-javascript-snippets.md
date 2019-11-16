---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1b08fbcb659a7a1ae381c29d1a575f1d7deb9f49
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636845"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const group = {
  description: "Self help community for library",
  displayName: "Library Assist",
  groupTypes: [
    "Unified"
  ],
  mailEnabled: true,
  mailNickname: "library",
  securityEnabled: false
};

let res = await client.api('/groups')
    .post(group);

```