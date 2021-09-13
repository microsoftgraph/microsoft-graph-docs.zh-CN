---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1bd4a0cb0c1fbaf1d9703b11c5dbafc0ce12973b61dc1d3f047e53e9eecf30ef
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218758"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const messageRule = {
    displayName: 'Important from partner',
    actions: {
        markImportance: 'high'
     }
};

await client.api('/me/mailFolders/inbox/messageRules/AQAAAJ5dZqA=')
    .update(messageRule);

```