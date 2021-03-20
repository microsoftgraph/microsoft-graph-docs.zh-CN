---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 02f43786b893334d109876d9a220286e189c4775
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50951371"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().schools("10001").classes("11001")
    .buildRequest()
    .delete();

```