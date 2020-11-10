---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 41bdf520b575e0b9a96b01105ce8eeaf9d1ca6bc
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48970098"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IUserFindRoomsCollectionPage findRooms = graphClient.me()
    .findRooms()
    .buildRequest()
    .get();

```