---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2d8dc3be0c13ceeb1fd82c57a783e5635fc53ac8
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48969226"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DriveItem driveItem = graphClient.shares("{shareIdOrUrl}").driveItem()
    .buildRequest()
    .get();

```