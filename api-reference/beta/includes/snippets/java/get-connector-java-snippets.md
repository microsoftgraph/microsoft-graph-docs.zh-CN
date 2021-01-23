---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d695c93eb13346cc1dd4baf45f90a0ca9df993bd
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2021
ms.locfileid: "49946255"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Connector connector = graphClient.onPremisesPublishingProfiles("applicationProxy").connectors("{id}")
    .buildRequest()
    .get();

```