---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e48cea7bd2f63c0425be75caefaaeb563e19cde7341480b4957aebc55fcef0bb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333408"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().profile().projects("{id}")
    .buildRequest()
    .delete();

```