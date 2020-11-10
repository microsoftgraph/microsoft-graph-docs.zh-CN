---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 91e4c6366e65a86adccec175bc3d596644203ec2
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48975659"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ITeamCollectionPage joinedTeams = graphClient.me().joinedTeams()
    .buildRequest()
    .get();

```