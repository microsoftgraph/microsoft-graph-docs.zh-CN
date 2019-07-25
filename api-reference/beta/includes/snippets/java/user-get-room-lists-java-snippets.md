---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f9c58376839980506a0e5c900be223e976ff9c38
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35867748"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IEmailAddressCollectionPage findRoomLists = graphClient.me()
    .findRoomLists()
    .buildRequest()
    .get();

```