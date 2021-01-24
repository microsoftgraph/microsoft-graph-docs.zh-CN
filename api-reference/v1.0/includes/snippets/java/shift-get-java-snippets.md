---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 96949a0701041973cc96a4c0ba50b8095cefbfc9
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2021
ms.locfileid: "49946269"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Content shiftPreferences = graphClient.users("871dbd5c-3a6a-4392-bfe1-042452793a50").shiftPreferences()
    .buildRequest()
    .get();

```