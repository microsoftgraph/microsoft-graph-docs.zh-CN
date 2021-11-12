---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c6b0e0626de0f5dc30b9e7eaff401b083a7322a6b15136819538641d5e190af4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218470"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PlannerUser plannerUser = graphClient.me().planner()
    .buildRequest()
    .get();

```