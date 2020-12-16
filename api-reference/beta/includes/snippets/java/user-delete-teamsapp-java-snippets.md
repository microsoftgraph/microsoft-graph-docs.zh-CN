---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d8c9d3c9ad0852d1b5b3d00bc3480b852a537db5
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "49692727"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.users("5b649834-7412-4cce-9e69-176e95a394f5").teamwork().installedApps("NWI2NDk4MzQtNzQxMi00Y2NlLTllNjktMTc2ZTk1YTM5NGY1IyNhNmI2MzM2NS0zMWE0LTRmNDMtOTJlYy03MTBiNzE1NTdhZjk")
    .buildRequest()
    .delete();

```