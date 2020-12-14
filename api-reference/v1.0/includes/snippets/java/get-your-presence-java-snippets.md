---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b5695720df9558277f83b7fb03ec0d072896ef3f
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/11/2020
ms.locfileid: "49663949"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Content presence = graphClient.me().presence()
    .buildRequest()
    .get();

```