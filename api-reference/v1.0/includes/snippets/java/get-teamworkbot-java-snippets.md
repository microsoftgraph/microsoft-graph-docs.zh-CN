---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9c1b8078f95f5a7c4e01d1f1a13a685600ff73f4
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50774783"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TeamworkBot teamworkBot = graphClient.appCatalogs().teamsApps("e4c5c249-bb4b-419e-b7c5-b1d98559368b").appDefinitions("ZTRjNWMyNDktYmI0Yi00MTllLWI3YzUtYjFkOTg1NTkzNjhiIyMyLjAuMSMjUHVibGlzaGVk").bot()
    .buildRequest()
    .get();

```