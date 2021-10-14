---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 34306a48f73d4e4c414b57f91e74bb10f90f6c96841abbd8b9091d8b370c79c6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219048"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.groups("02bd9fd6-8f93-4758-87c3-1fb73740a315").conversations("AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgAQABuXO3guDWBMpyKF7LsVwfU=")
    .buildRequest()
    .delete();

```