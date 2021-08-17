---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4c993b0c2f1592c607a95e245d0a5bb103ee12f7d01c8c8cf54acc5d37c04161
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278538"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const group = {
  description: 'Self help community for library',
  displayName: 'Library Assist',
  groupTypes: [
    'Unified'
  ],
  mailEnabled: true,
  mailNickname: 'library',
  securityEnabled: false
};

await client.api('/groups')
    .post(group);

```