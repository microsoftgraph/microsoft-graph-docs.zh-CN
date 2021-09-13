---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 11906cb6baf6dd7300bc00cd346e335bb29ca28af6c8512834efe505c5c5f139
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332778"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.groups("{id}").appRoleAssignments("{id}")
    .buildRequest()
    .delete();

```