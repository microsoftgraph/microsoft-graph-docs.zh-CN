---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1b71de7d02f030bbf71121f43cc9a71eefa5d200
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35867705"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IEmailAddressCollectionPage findRooms = graphClient.me()
    .findRooms()
    .buildRequest()
    .get();

```