---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a9d7d15f849a8cef61f86b350ad137c04e46d117
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/17/2021
ms.locfileid: "50274675"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDirectoryObjectCollectionWithReferencesPage appliesTo = graphClient.policies().tokenIssuancePolicies("{id}").appliesTo()
    .buildRequest()
    .get();

```