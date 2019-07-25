---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 4d8c6b108a6ed5c879d13290e335b1fd8b26cedd
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35890141"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

boolean securityEnabledOnly = True;

graphClient.directoryObjects("{object-id}")
    .getMemberGroups(securityEnabledOnly)
    .buildRequest()
    .post();

```