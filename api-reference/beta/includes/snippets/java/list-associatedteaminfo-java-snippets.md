---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cde9817224f1824be24a41cb1399c7a0887a7a3e
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65203693"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AssociatedTeamInfoCollectionPage associatedTeams = graphClient.me().teamwork().associatedTeams()
    .buildRequest()
    .get();

```