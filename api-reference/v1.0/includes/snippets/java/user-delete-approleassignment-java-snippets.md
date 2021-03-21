---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b32e5d4c7b1adc4c7f0ca957dc664e5a80a0dc09
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50969121"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.users("{id}").appRoleAssignments("{id}")
    .buildRequest()
    .delete();

```