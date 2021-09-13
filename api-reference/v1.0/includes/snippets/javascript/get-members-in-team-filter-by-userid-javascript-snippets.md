---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 18f65412fbe28211697fae8bc674242de4805d2283fe59e545b0bb50cb4ac6eb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161978"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let members = await client.api('/teams/ee0f5ae2-8bc6-4ae5-8466-7daeebbfa062/members')
    .filter('(microsoft.graph.aadUserConversationMember/userId eq \'73761f06-2ac9-469c-9f10-279a8cc267f9\')')
    .get();

```